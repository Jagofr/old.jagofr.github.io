<style>
.header-bar {
    position: sticky;
    z-index: 99;
    background: white;
    top: 0;
    display: flex;
    width: 100%;
}
.header-bar * {
    padding: 1rem;
}
.header-bar__spacer {
    margin-left: auto;
}
.header-bar__link {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 0;
}
.header-bar__more-links {
    display: inline-flex;
    max-width: min-content;
    max-height: min-content;
    margin-top: auto;
    margin-bottom: auto;
    flex-flow: column nowrap;
}
.header-bar__more-links_leftSpace {
    margin-left: auto;
    margin-right: 0;
}
.header-bar__more-links_rightSpace {
    margin-right: auto;
    margin-left: 0;
}
.more-links__line {
    background: black;
    width: 1rem;
    height: 0.125rem;
    padding: 0;
}
.more-links__line.two {
    margin-top: 0.25rem;
    margin-bottom: 0.25rem;
}
.link__nuxt {
    height: 100%;
    display: flex;
    align-items: center;
}

</style>

<template>
    <div class="header-bar">
        <span class="header-bar__link" style="padding: 0;">
            <NuxtLink to="/" class="link__nuxt" style="text-decoration: none;"><h1 style="padding: 0;">I am the header! Really, I am!</h1></NuxtLink>
        </span>
        <div class="header-bar__spacer"></div>
        <span class="header-bar__link">
            <h1>Jagofr's Website!</h1>
        </span>
        <div class="header-bar__spacer"></div>
        <span class="header-bar__link">
            <NuxtLink to="/blog" class="link__nuxt">Blog</NuxtLink>
        </span>
        <span class="header-bar__link">
            <NuxtLink to="/socials" class="link__nuxt">Socials</NuxtLink>
        </span>
        <span class="header-bar__link">
            <NuxtLink to="/about" class="link__nuxt">About</NuxtLink>
        </span>
        <button class="header-bar__more-links header-bar__more-links" hidden>
            <span class="more-links__line one"></span>
            <span class="more-links__line two"></span>
            <span class="more-links__line three"></span>
        </button>
    </div>
</template>

<script>

</script>