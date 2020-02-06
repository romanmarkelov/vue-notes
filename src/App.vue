<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->

    <aside class="sidebar"></aside>
    <main class="content">
      <router-view />
    </main>
  </div>
</template>

<style lang="scss">
/* Box sizing rules */
*,
*::before,
*::after {
  box-sizing: border-box;
}

/* Remove default margin */
body,
h1,
h2,
h3,
h4,
p,
ul[class],
ol[class],
li,
figure,
figcaption,
blockquote,
dl,
dd {
  margin: 0;
}

body {
  background-color: #faf9fa;
  font-family: 'Open Sans', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  min-height: 100vh;
  scroll-behavior: smooth;
  text-rendering: optimizeSpeed;
  line-height: 1.5;
}

#app {
  display: flex;
  margin: 0 auto;
}

h1 {
  margin-bottom: 20px;
  color: #211551;
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

.content {
  width: 960px;
  margin: 0 auto;
  padding: 0 15px;
}

.sidebar {
  height: 100vh;
  margin-right: auto;
  flex: none;
  width: 74px;
  background-color: #fff;
  border-right: 1px solid #f0eff2;
}
</style>
