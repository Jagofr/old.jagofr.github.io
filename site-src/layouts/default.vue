<template>
    <HeaderComponent />
    <div class="content-body">
        <LazyNuxtPage />
    </div>
    <FooterComponent />
</template>

<script>

</script>

<style>
    .header-bar {
        margin-bottom: auto;
    }
    .footer-bar {
        margin-top: auto;
    }
    .content-body .body {
        display: flex;
        width: 100%;
        align-items: center;
        justify-content: center;
        min-height: min-content;
        flex-flow: column nowrap;
        font-family: sans-serif;
    }
    .content-body .body > * {
        padding: 1.75rem;
    }
</style>