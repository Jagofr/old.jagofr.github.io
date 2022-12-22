<style lang="less">
@import "~/assets/jCss/layout/navbar";
</style>

<template lang="pug">
nav.nav-bar 
  .nav-bar__menu-btn-box
    button.nav-bar__menu-btn 
      span.nav-bar__menu-btn-icon
        i.las.la-bars 
  .nav-bar__header
    span.nav-bar__header_text 
      NuxtLink(to="/").nav-bar__link Jagofr
  .nav-bar__social-links
    span.nav-bar__links_item
      a(href="https://github.com/Jagofr/jagofr.github.io/").nav-bar__link
        i.lab.la-github
    span.nav-bar__links_item
      a(href="http://www.avato.media/").nav-bar__link
        i.las.la-globe
    span.nav-bar__links_item
      a(href="https://linkedin.com/in/Jagofr").nav-bar__link
        i.lab.la-linkedin-in 
    span.nav-bar__links_item
      a(href="https://wa.me/+18768309280/").nav-bar__link
        i.fab.fa-whatsapp
  .nav-bar__links.hidden
    span.nav-bar__links_item 
        NuxtLink(to="/blog").nav-bar__link Blog
    span.nav-bar__links_item
        NuxtLink(to="/socials").nav-bar__link Socials
    span.nav-bar__links_item 
        NuxtLink(to="/about").nav-bar__link About  
</template>

<script setup>
onMounted(() => {
    let mobileMenuBtn = document.querySelector("button.nav-bar__menu-btn");
    let mobileMenu = document.querySelector("div.nav-bar__links");
    let mobileMenuItems = document.querySelectorAll(".nav-bar__link");

    mobileMenuBtn.addEventListener("click", (event) => {    
        event.preventDefault();
        mobileMenu.classList.toggle("hidden");
    })

    mobileMenuItems.forEach((item) => {
        item.addEventListener("click", (event) => {
            mobileMenu.classList.toggle("hidden", true);
        })
    })

});
</script>