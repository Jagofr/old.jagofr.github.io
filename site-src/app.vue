<style>
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
