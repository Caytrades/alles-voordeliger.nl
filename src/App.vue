<script setup>
import { RouterLink, RouterView} from 'vue-router'
</script>

<template>
  <header class="header">
    <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
  </header>

    <RouterView/>

</template>

<style scoped>
.header{
padding: 20px;
background-color: #F2C075;
margin-bottom: 20px;
border-radius: 10px;
}

nav{
  display: flex;
  gap: 20px;
}

nav a.router-link-exact-active{
  text-decoration: none;
  color: white;
}

nav a.router-link-exact-active:hover{
  color: grey;
  transition: ease 0.5s;
}


nav a{
  text-decoration: none;
  color: white;
}

nav a:hover{
  color: grey;
  transition: ease 0.5s;
}

</style>
