<script setup>
const { data: posts, pending } = await useFetch('https://jsonplaceholder.typicode.com/posts?_limit=3')
</script>

<template>
  <main>
    <h1>Nuxt 4 Testlauf</h1>
    <div v-if="pending">Lädt...</div>
    <ul v-else>
      <li v-for="post in posts" :key="post.id">
        <strong>{{ post.title }}</strong>
      </li>
    </ul>
    
    <AppAlert>Nuxt 4 läuft im Kompatibilitätsmodus!</AppAlert>
  </main>
</template>