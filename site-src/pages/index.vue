<script setup>

definePageMeta({
    layout: "index",
});

onMounted(() => {
    let hiddenItems = document.querySelectorAll(".fade-out");
    hiddenItems.forEach((x) => {
        x.classList.toggle("fade-out", false);
    })
});
</script>
<template lang="pug">
.body
    .jumbo
        .grid_2x2.vh.mobile
            .top.left#personal-intro 
                .grid_2x2.stretch
                    .bottom.span.flex.inline.columns.pad_2xX.flex_end_align
                        h1.text_reset Hi! My name is Gerard.
                        h2.text_reset I also go by "Jagofr".
            .top.right
                .flex.inline.columns.stretch.pad_2x.flex_end_justify.flex_gap_sm.flex_start_justify_mobileOnly
                    h3.text__align_center_mobileOnly Who am I?
                    p.text__align_justify_mobileOnly 
                        | I'm Gerard Francis, or Jamie if you feel more endearing. I am a freelance,
                        | full-stack web/mobile/app developer, who (at least right now) focuses on cross-platform,
                        | mobile-first websites and web applications. I typically use some JavaScript stack of sorts.
                        | Currently, I'm using Nuxt.js to develop this Website as a Jamstack/SSG (or simply static)
                        | webpage! But I also use PHP for my company site, 
                        a(href="http://www.avato.media/") AVATO Media
                        |.
            .bottom.left
                .flex.inline.columns.stretch.pad_2x.text__align_center.flex_gap_lg
                    h3 This site's status...
                    p.text__align_justify   
                        | Right now, if I haven't updated this yet again, this page may just be a basic layout. But I'm still working
                        | on it! I moved all the lorems to the 
                        NuxtLink(to="/tests") tests page
                        |  so that the actual pages can get some room to breathe! Hope you like how it is so far though; and please feel
                        | free to use that 
                        a(href="https://github.com/Jagofr/jagofr.github.io/") GitHub link
                        |  up there to check out the source code for this site! Have fun!
            .bottom.right(style="padding: 0;")
                .flex.inline.columns.stretch.pad_2x.flex_gap_lg
                    h3.text__align_left.pad_smX Latest Blog Articles 
                    .grid_2x2.stretch 
                        a(href="/blog").btn-link.top.left.flex.inline.flex_center Blog Post 1
                        a(href="/blog/test").btn-link.top.right.flex.inline.flex_center Blog Post 2
                        a(href="/blog").btn-link.bottom.left.flex.inline.flex_center Blog Post 3
                        a(href="/blog/test").btn-link.bottom.right.flex.inline.flex_center Blog Post 4


</template>
<style lang="less">
@import "~/assets/jCss/partials/_jCssVars.less";
#personal-intro {
    background-image: url("/img/jamie-13.jpg");
    background-size: 100%;
    background-position-y: 30%;
    color: @light-700;
    text-shadow: 4px 4px 6px @dark-700;
}

@media only screen and (max-width: 900px) {
    .grid_2x2.vh {
        & div:nth-child(even) {
            background-color: @dark-500;
            color: @light-500;
        }
    }
}

@media only screen and (min-width: 900px) {
    .grid_2x2.vh {
         >.top.right, >.bottom.left {
            background-color: @dark-500;
            color: @light-500;
        }

        >.left {
            padding-left: 10rem;
        }
        >.right {
            padding-right: 10rem;
        }
    }
}
</style>