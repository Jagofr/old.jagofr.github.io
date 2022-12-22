<style>
@import url(https://cdnjs.cloudflare.com/ajax/libs/line-awesome/1.3.0/line-awesome/css/line-awesome.min.css);
@import url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/fontawesome.min.css);
@import url(https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/brands.min.css);


*, *:before, *:after {
  box-sizing: border-box;
}
* {
  margin: 0;
  padding: 0;
  transition: all 200ms ease-in-out, transform 650ms ease-in-out;
}
[hidden] {
  display: none !important;
}

#app{
  min-height: 100vh;
  display: block;
}
</style>

<template>
  <div id="app">
    <NuxtLayout />
  </div>
</template>

<script setup>
useHead({
  meta: [{
    name: 'viewport',
    content: "width=device-width, initial-scale=1.0"
  }, {
    charset: "utf-8"
  }, {
    "http-equiv": "x-ua-compatible",
    content: "IE=edge"
  }]
});
</script>
