<template>
    <img id="photo" :src="photo" alt="photo de profil" class="photo" />

    <h1> <span id="prenom">{{ prenom }}</span> <span id="nom">{{ nom }}</span>
    </h1>

</template>

<script>
export default {
    data() {
        return {
            nom: "Laroche",
            prenom: "Pierre",
            photo: "https://randomuser.me/api/portraits/men/79.jpg",
        };
    },
};
</script>

<style scoped>
.photo {
    display: block;
    border-radius: 50%;
    margin: 10px auto;
    width: 150px;
    height: 150px;
}
</style>