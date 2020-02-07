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
@import '@/assets/scss/main.scss';
</style>
