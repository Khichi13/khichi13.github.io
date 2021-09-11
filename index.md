---
layout: default
title: Vive La Mystique
description: This is a random website for you to waste your time.
keywords: portfolio, farooq khichi, freelancer
drawer: true
---

<div class="col-md-8">
  
I'm the <b>hero of a thousand stories</b>. I'm a superhero, an assassin, a soldier!
I've slain dragons and traveled through portals. I am a spartan, a commander, a king!
I've saved a thousand worlds and countless more lives. What am I? I'm a gamer!

## My Gigs

{% include list_services.html %}

</div>

<div class="col-md-4">

![Slytherin House logo](https://github.com/Khichi13/khichi13.github.io/blob/main/assets/images/slytherin.png)
  
<section class="mdc-card mdc-card--outlined highlighted">
  <div class="mdc-card__content">

## Blog Posts
    
{% include list_posts.html %}

  </div>
</section>

{% include widget_goodreads.html %}

</div>

<!-- PWA -->
<script src="{{ site.baseurl }}/assets/scripts/webapp.js"></script>
<script type="module">
  import 'https://cdn.jsdelivr.net/npm/@pwabuilder/pwaupdate';
  const el = document.createElement('pwa-update');
  document.body.appendChild(el);
</script>
<script>
  function install() {
    const ref = document.getElementById("a2hs");
    if (!ref.getInstalledStatus()) {
      ref.openPrompt();
    } else {
      showSnackbar("You have already installed the app.");
    }
  }
</script>
