<template>
    <HeaderComponent />
    <div class="content-body">
        <LazyNuxtPage />
    </div>
    <FooterComponent />
</template>

<style lang="less">
@import "~/assets/jCss/layout/main.less"; 
.content- { 
    &body {    
        .body {
            display: flex;
            width: 100%;
            align-items: center;
            justify-content: center;
            min-height: min-content;
            flex-flow: column nowrap;
            font-family: sans-serif;
            text-align: justify;
        }
    } 
    @media only screen and (min-width: 900px) {
        &body {
            padding: 0 @desktop-navPad;
        }
    }
}
</style>