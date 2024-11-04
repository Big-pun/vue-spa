<template>
    <img id="photo" :src="photo" :alt="propNom" class="photo" />

    <h1> {{ propNom }}
    </h1>

</template>

<script>
export default {
    props: ['propNom'],
    data() {
        return {
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