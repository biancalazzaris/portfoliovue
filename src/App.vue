<template>
  <div>
    <Navbar />
    <div id="app">
      <nav>
        <router-link to="/">Home</router-link> |
        <router-link to="/sobre">Sobre</router-link> |
        <router-link to="/education">Education</router-link> |
        <router-link to="/jobs">Jobs</router-link> |
        <router-link to="/contact">Contact</router-link>
      </nav>
      <router-view />
    </div>
  </div>
</template>

<script>
import Navbar from '@/components/Navbar.vue';

export default {
  components: {
    Navbar,
  },
};
</script>

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
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
