<template>
  <nav>
    <router-link to="/">Home</router-link> |
    <!-- by binding routes in the style below if path is going to be change in future it will still going to works -->
    <router-link :to="{ name: 'about' }">About</router-link> |
    <router-link :to="{ name: 'job' }">Jobs</router-link>
  </nav>
  <router-view />
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

nav {
  padding: 30px;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding: 10px;
  border-radius: 5px;
}

nav a.router-link-exact-active {
  color: white;
  background-color: crimson;
}
</style>
