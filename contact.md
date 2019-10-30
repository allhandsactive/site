---
title: "Contact Us"
layout: splash
permalink: /contact
header:
  overlay_color: "#000"
  overlay_filter: "0.4"
  overlay_image: /assets/images/contact-splash.jpg
  actions:
    - label: "Become a Member"
      url: "/membership"
    - label: "Donate"
      url: "https://www.gofundme.com/f/aha-2019-2020-fundraiser"
  caption: "Photo by [**Nicolas Thomas**](https://unsplash.com/@nicolasthomas?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [**Unsplash**](https://unsplash.com)"
excerpt: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Cras malesuada scelerisque mauris sit amet aliquet. Mauris consectetur tincidunt quam quis laoreet."

intro: 
  - title: Want to Know More?
    excerpt: "Send us an email and we'll get back to you as soon as possible!"
---

{% include feature_row id="intro" type="center" %}

<form action="#" style="width: 50%">
  <input type="text" name="first_name" placeholder="Jane" aria-label="first name" style="width: 46.5%; float: left; margin-bottom: 1em" />
  <input type="text" name="last_name" placeholder="Smith" aria-label="last name" style="width: 46.5%; float: right; margin-bottom: 1em" />
  <input type="email" name="email" aria-label="email" style="margin-bottom: 1em" placeholder="john.smith@gmail.com" />
  <textarea cols="46" rows="5" name="comments" aria-label="comments" style="margin-bottom: 1em" placeholder="Send us a message"></textarea>
  <input class="btn btn--primary" type="submit" value="Submit" />
</form>
{: .align-center}