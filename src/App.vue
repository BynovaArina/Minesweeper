<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
#app {
  max-width: 600px;
  width: 100%;
  margin: 10rem auto;
  background: #111;
}

html, body {
  margin: 0;
  width: 100%;
  height: 100%;
}

html {
  font-size: 62.5%;
}

body {
  min-height: 100vh;
  font-size: 1.8rem;
  line-height: 1.6;
  color: #eee;
  
  background-color: #000;
  background-image: url('data:image/svg+xml,%3Csvg xmlns="http://www.w3.org/2000/svg" width="36" height="72" viewBox="0 0 36 72"%3E%3Cg fill-rule="evenodd"%3E%3Cg fill="%239C92AC" fill-opacity="0.1"%3E%3Cpath d="M2 6h12L8 18 2 6zm18 36h12l-6 12-6-12z"/%3E%3C/g%3E%3C/g%3E%3C/svg%3E');
  
  animation-name: bg;
  animation-duration: 60s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  animation-direction: alternate;
  
  -webkit-font-smoothing: antialiased;
  text-rendering: optimizeLegibility;
  -moz-osx-font-smoothing: grayscale
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
