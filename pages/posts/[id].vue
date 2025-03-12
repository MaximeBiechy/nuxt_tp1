<script setup lang="ts">
const route = useRoute()

const id = route.params.id;
</script>

<template>
  <div class="container">
    <div v-if="id === '1'">
      <NuxtLink to="/posts/2" class="link">C’est l’heure du duel</NuxtLink>
    </div>
    <div v-else-if="id === '2'">
      <NuxtLink to="/posts/1" class="link">En avant Pikachu</NuxtLink>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  gap: 1rem;
  margin-top: 5rem;
}

.link {
  color: black;
  text-decoration: none;
  padding: 0.5rem 1rem;
  border: 1px solid black;
  border-radius: 0.25rem;
}
</style>
