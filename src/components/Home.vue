<script setup>
import { ref, provide } from 'vue';

const animal = ref("");
provide('animalKey', animal);

</script>



<template>
  <div>
    <RouterLink to="/Liste/chien">CHIEN</RouterLink>
  </div>
  <div>
    <RouterLink to="/Liste/chat">CHAT</RouterLink>
  </div>
  <div>
    <RouterLink to="/Liste/tortue">TORTUE</RouterLink>
  </div>
  <div>
    <RouterLink to="/Liste/yeti">YETI</RouterLink>
  </div>
  <br>
  <br>
  <br>
  <div>
    <RouterLink to="/Panier">PANIER</RouterLink>
  </div>
</template>




<style scoped>
header {
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

nav {
  width: 100%;
  font-size: 12px;
  text-align: center;
  margin-top: 2rem;
}

nav a.router-link-exact-active {
  color: var(--color-text);
}

nav a.router-link-exact-active:hover {
  background-color: transparent;
}

nav a {
  display: inline-block;
  padding: 0 1rem;
  border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
  border: 0;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }

  nav {
    text-align: left;
    margin-left: -1rem;
    font-size: 1rem;

    padding: 1rem 0;
    margin-top: 1rem;
  }
}

div {
  background-color: rgb(248, 248, 248);
  color: white;
  padding: 1rem;
  margin-bottom: 1rem;
}
</style>
