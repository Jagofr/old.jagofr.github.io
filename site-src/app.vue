<style>
@import url(https://cdnjs.cloudflare.com/ajax/libs/semantic-ui/2.5.0/semantic.min.css);
@import url(https://cdnjs.cloudflare.com/ajax/libs/line-awesome/1.3.0/line-awesome/css/line-awesome.min.css);


*, *:before, *:after {
  box-sizing: border-box;
}
* {
  margin: 0;
  padding: 0;
}
[hidden] {
  display: none !important;
}

#app{
  min-height: 98vh;
  display: flex;
  flex-flow: column;
  align-items: center;
  justify-content: center;
}
</style>

<template>
  <div id="app">
    <NuxtLayout />
  </div>
</template>
