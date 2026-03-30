<template>
  <div class="page">
    <h1>🏠 Startseite</h1>
    <p>Willkommen zu meinem Nuxt 4 Test.</p>
    
    <NuxtLink to="/helloWorld" class="btn">
      Gehe zur Hello World Seite →
    </NuxtLink>
  </div>
</template>

<style scoped>
.page { font-family: sans-serif; padding: 2rem; }
.btn {
  display: inline-block;
  padding: 10px 20px;
  background-color: #00dc82; /* Nuxt Green */
  color: white;
  text-decoration: none;
  border-radius: 5px;
  font-weight: bold;
}
</style>