<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div id="layout">
    <header>
      <div class="wrapper">
        <nav>
          <RouterLink to="/">Event</RouterLink> |
          <RouterLink to="/event-list-view">Event list View</RouterLink>
        </nav>
      </div>
    </header>

    <RouterView />
  </div>
</template>

<style>
#layout {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
nav {
  padding: 20px;
}
nav a {
  font-weight: bold;
  color: #42b983;
  text-decoration: none;
}
nav a.router-link-exact-active {
  color: #35495e;
}
h2 {
  font-size: 20px;
}
</style>
