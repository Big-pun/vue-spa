<script>
  export default {
    data() {
      return {
        nom: "John doe"
      }
    }
  }
</script>

<template>
  <h1>Bonjour {{ nom }}</h1>

</template>

<style>
  h1 {
    color: green;
  }

</style>
