---
layout: post
permalink: /implementing-open-graph-meta-tags-in-2sxc
title: Coding Open Graph meta tags for 2sxc apps
path: 2015-5-28-Implementing-Open-Graph-Meta-Tags-In-2sxc.md
tags:
- opengraph
- 2sxc
- metatags
- seo
published: true
---

For one of the projects i was working on i had to figure out a way to create Open Graph meta tags.  
Website i was working on is [Croatia Boat Charter](http://croatiaboatcharter.com/), it is a website for chater agency Plavetnilo d.o.o, their primary service is renting yachts.  
Every yacht had a corresponding detail page and information about yacht (name, model, description etc..) had to be included inside those meta tags.  
Whole website was implemented using DotNetNuke and 2SexyContent module for DNN.

Example code:
<pre>
@using System.Web.UI.HtmlControls;
</pre>

{% highlight C# %}

@{
  Page page = HttpContext.Current.Handler as Page;
  DotNetNuke.Framework.CDefault tp = (DotNetNuke.Framework.CDefault)page;
  if (tp != null)
  {
      //page.Title = Content.MetaTitle;
      //tp.Description = Content.MetaDescription;
  }

  // change existing meta tag
  HtmlMeta metaDescription = (HtmlMeta)page.FindControl("metaDescription");
  metaDescription.Visible = true;
  //metaDescription.Content = "TestMe";
  //metaDescription.Content = Content.MetaDescription;

  /* Set Open Graph Meta tags */

  if (page != null)
  {
      // og:site_name
      HtmlMeta metaOgSiteName = new HtmlMeta();
      metaOgSiteName.Attributes.Add("property", "og:site_name");
      metaOgSiteName.Content = String.Format("{0}", "Croatia boat charter");
      page.Header.Controls.Add(metaOgSiteName);

      // og:url
      HtmlMeta metaOgUrl = new HtmlMeta();
      metaOgUrl.Attributes.Add("property", "og:url");
      metaOgUrl.Content = String.Format("{0}", friendlyUrl);
      page.Header.Controls.Add(metaOgUrl);

      // og:title
      HtmlMeta metaOgTitle = new HtmlMeta();
      metaOgTitle.Attributes.Add("property", "og:title");
      metaOgTitle.Content = String.Format("{0} {1}", yachtDetail.YachtProducerName, yachtDetail.ModelName);
      page.Header.Controls.Add(metaOgTitle);
  }

  if (page != null && !String.IsNullOrEmpty(yachtDetail.Description))
  {
      // og:description
      HtmlMeta metaOgDesc = new HtmlMeta();
      metaOgDesc.Attributes.Add("property", "og:description");
      metaOgDesc.Content = String.Format("{0}", yachtDetail.Description);
      page.Header.Controls.Add(metaOgDesc);
  }


  if (page != null)
  {
      // og:image
      HtmlMeta metaOgImage = new HtmlMeta();
      metaOgImage.Attributes.Add("property", "og:image");
      metaOgImage.Content = String.Format(photosSrc, photosUrl, yachtDetail.YachtID, 0);
      page.Header.Controls.Add(metaOgImage);

      // og:type
      HtmlMeta metaOgType = new HtmlMeta();
      metaOgType.Attributes.Add("property", "og:type");
      metaOgType.Content = String.Format("{0}", "website");
      page.Header.Controls.Add(metaOgType);
  }

  /* Create new meta tag with name & content and add to header */
  /* Set Twitter Card Meta tags */

  if (page != null)
  {
      // twitter:site
      HtmlMeta metaTwitterSite = new HtmlMeta();
      metaTwitterSite.Name = "twitter:site";
      metaTwitterSite.Content = String.Format("{0}", "@CroatiaBoat");
      //meta.Scheme = "YYYY-MM-DD";
      page.Header.Controls.Add(metaTwitterSite);

      // twitter:url
      HtmlMeta metaTwitterUrl = new HtmlMeta();
      metaTwitterUrl.Name = "twitter:url";
      metaTwitterUrl.Content = String.Format("{0}", friendlyUrl);
      page.Header.Controls.Add(metaTwitterUrl);

      // twitter:title
      HtmlMeta metaTwitterTitle = new HtmlMeta();
      metaTwitterTitle.Name = "twitter:title";
      metaTwitterTitle.Content = String.Format("{0} {1} {2}", yachtDetail.YachtProducerName, yachtDetail.ModelName, "- Croatia boat charter");
      page.Header.Controls.Add(metaTwitterTitle);
  }

  if (page != null && !String.IsNullOrEmpty(yachtDetail.Description))
  {
      // twitter:description
      HtmlMeta metaTwitterDescription = new HtmlMeta();
      metaTwitterDescription.Name = "twitter:description";
      metaTwitterDescription.Content = String.Format("{0}", yachtDetail.Description);
      page.Header.Controls.Add(metaTwitterDescription);
  }


  if (page != null)
  {
      // twitter:image
      HtmlMeta metaTwitterImage = new HtmlMeta();
      metaTwitterImage.Name = "twitter:image";
      metaTwitterImage.Content = String.Format(photosSrc, photosUrl, yachtDetail.YachtID, 0);
      page.Header.Controls.Add(metaTwitterImage);

      // twitter:card
      HtmlMeta metaTwitterCard = new HtmlMeta();
      metaTwitterCard.Name = "twitter:card";
      metaTwitterCard.Content = String.Format("{0}", "summary_large_image");
      page.Header.Controls.Add(metaTwitterCard);
  }

}

{% endhighlight %}


