<template>
  <div id="app">
    <div class="carte">
      <Identification />
      <Coordonnées />
      <Hobbies />
    </div>

  </div>
</template>

<script>
import Identification from './components/Identification.vue'
import Coordonnées from './components/Coordonnées.vue'
import Hobbies from './components/Hobbies.vue'


export default {
  components: {
    Identification,
    Coordonnées,
    Hobbies

  }
}
</script>



<style>
.carte {
  width: 300px;
  border-radius: 5px;
  padding: 10px;
  border: 1px solid black;
  color: white;
  margin: 0 auto;
  background-color: rgb(39, 33, 81);
}

.carte h1 {
    text-align: center;
    border-bottom: 1px solid white;
    margin-bottom: 10px;
}

.carte h3 {
    text-align: center;
}
</style>
