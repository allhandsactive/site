---
layout: splash
permalink: /
header:
  overlay_color: "#000"
  overlay_filter: "0.6"
  overlay_image: /assets/images/ahayarn.jpg
  actions:
    - label: "Visit"
      url: "/visit"
    - label: "Donate"
      url: "/donate"
excerpt: "Ann Arbor's all-volunteer non-profit community makerspace."

feature_row1:
  - title: "What is a makerspace?"
    image_path: assets/images/mural-landscape.jpg
    alt: "AHA mural with keyboard, star, needle, wrench and soldering iron"
    excerpt: "All Hands Active (AHA!) is a place to <b><i>learn by doing</i></b> with a
      welcoming and supportive <b><i>community</i></b>. AHA! is Ann Arbor's original
      hackerspace and makerspace."
    url: "/about"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_row2:
  - image_path: assets/images/somehandsactive.jpg
    alt: "People gathered to do arts and crafts"
    title: "Interested? Come on by!"
    excerpt: "Visit us during public hours, bring your project, or take a class! We always have volunteering opportunities and are
      always accepting new members."
    url: "/visit"
    btn_label: "Read More"
    btn_class: "btn--primary"

---

{% include feature_row id="feature_row1" type="left" %}

{% include feature_row id="feature_row2" type="right" %}

## Subscribe
{: .text-center}

Join our announcements email list!
{: .text-center}

{% include mailchimp-form.html %}
