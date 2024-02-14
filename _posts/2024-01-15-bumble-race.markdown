---
layout: post
title: Bumble Race
date: 2024-01-15 13:00:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
fig-caption: # Add figcaption (optional)
img: we-in-rest.jpg
---

<!-- Youtube Videos -->
<div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; margin-bottom: 20px;">
  <iframe style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;" src="https://www.youtube.com/embed/TBCRlnwJtZU" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<!-- Game Images -->
<div class="carousel-container" style="max-width: 100%; overflow: hidden; display: flex; cursor: grab;">
  <div class="carousel-slide" style="display: flex; transition: 0.5s all ease-in-out; margin-right: -10px;">
    <img src="{{ '/assets/img/dummy.jpg' | prepend: site.baseurl }}" alt="Açıklama1" style="width: calc(33.33% - 10px); margin-right: 10px; height: auto;">
    <img src="{{ '/assets/img/dummy.jpg' | prepend: site.baseurl }}" alt="Açıklama2" style="width: calc(33.33% - 10px); margin-right: 10px; height: auto;">
    <img src="{{ '/assets/img/dummy.jpg' | prepend: site.baseurl }}" alt="Açıklama3" style="width: calc(33.33% - 10px); margin-right: 10px; height: auto;">
    <img src="{{ '/assets/img/dummy.jpg' | prepend: site.baseurl }}" alt="Açıklama3" style="width: calc(33.33% - 10px); margin-right: 10px; height: auto;">
  </div>
</div>

<script>
document.addEventListener('DOMContentLoaded', function () {
  const slider = document.querySelector('.carousel-slide');
  let isDown = false;
  let startX;
  let scrollLeft;

  slider.addEventListener('mousedown', (e) => {
    isDown = true;
    slider.classList.add('active');
    startX = e.pageX - slider.offsetLeft;
    scrollLeft = slider.scrollLeft;
  });

  slider.addEventListener('mouseleave', () => {
    isDown = false;
    slider.classList.remove('active');
  });

  slider.addEventListener('mouseup', () => {
    isDown = false;
    slider.classList.remove('active');
  });

  slider.addEventListener('mousemove', (e) => {
    if (!isDown) return;
    e.preventDefault();
    const x = e.pageX - slider.offsetLeft;
    const walk = (x - startX) * 3; // 3: Kaydırma hızı, ihtiyaca göre ayarlanabilir
    slider.scrollLeft = scrollLeft - walk;
  });

  // Dokunmatik cihazlar için ekleyin
  slider.addEventListener('touchstart', (e) => {
    isDown = true;
    startX = e.touches[0].pageX - slider.offsetLeft;
    scrollLeft = slider.scrollLeft;
  });

  slider.addEventListener('touchend', () => {
    isDown = false;
  });

  slider.addEventListener('touchmove', (e) => {
    if (!isDown) return;
    const x = e.touches[0].pageX - slider.offsetLeft;
    const walk = (x - startX) * 3; // Dokunmatik cihazlarda da kaydırma hızı
    slider.scrollLeft = scrollLeft - walk;
  });
});
</script>


## About Game

Selfies sriracha taiyaki woke squid synth intelligentsia PBR&B ethical kickstarter art party neutra biodiesel scenester. Health goth kogi VHS fashion axe glossier disrupt, vegan quinoa. Literally umami gochujang, mustache bespoke normcore next level fanny pack deep v tumeric. Shaman vegan affogato chambray. Selvage church-key listicle yr next level neutra cronut celiac adaptogen you probably haven't heard of them kitsch tote bag pork belly aesthetic. 