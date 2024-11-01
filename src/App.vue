<template>
  <div id="app">
    <div class="carte">
      <Identification :nom="nom" />
      <Coordonnées />
      <Hobbies />
    </div>

    <button @click=changerNom()>Changer le nom</button>
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
  },
  data() {
    return {
      nom: "Laroche",
      prenom: "Pierre",
    };
  },
  methods: {
    changerNom() {
      const nouveauNom = prompt("Entrez un nouveau nom");
      if (nouveauNom) {
        this.nom = nouveauNom;
        console.log(this.nom);
        
      }
    },
  },
}
</script>



<style>
.carte {
  width: 300px;
  border-radius: 10px;
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
