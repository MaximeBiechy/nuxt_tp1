<template>
  <div>
    <NuxtRouteAnnouncer/>
    <div class="container">
      <NuxtLink to="/" class="link">Accueil</NuxtLink>
      <NuxtLink to="/bonjour" class="link">Bonjour</NuxtLink>
      <NuxtLink to="/profil" class="link">Profil</NuxtLink>
      <NuxtLink to="/posts/1" class="link">Posts</NuxtLink>
    </div>
    <img src="~/assets/img/logo.svg" alt="logo"/>
    <NuxtPage/>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-top: 1rem;
}

.link {
  color: black;
  text-decoration: none;
  padding: 0.5rem 1rem;
  border: 1px solid black;
  border-radius: 0.25rem;
}

img {
  display: block;
  margin: 2rem auto 0;
  width: 200px;
}
</style>
<script setup lang="ts">
</script>
