<template>
  <div>
    <h1>Welcome to nuxt 3</h1>
    <p>Hi {{ name }}, this is a simple example of a Nuxt 3 app</p>
  </div>
</template>

<script setup>
// get name from the query string
const route = useRoute()
const name = route.query.name || 'there'
</script>

<style>
body {
  font-family: 'Arial';
}
h1 {
  color: green;
}
</style>
