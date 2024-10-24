<template>
    <h3 id="email">{{ email }}</h3>
    <h3>{{ telephone }}</h3>
    <h3>{{ adresse.numero }} {{ adresse.rue }} <br>
        <span id="ville">{{ adresse.ville }}</span> {{ adresse.province }} <br>
        {{ adresse.codePostal }}
    </h3>
</template>

<script>
export default {
    data() {
        return {
            email: "pierrel@mail.com",
            telephone: "819-965-7410",
            adresse: {
                numero: "1585",
                rue: "Rue des pins",
                ville: "Trois-Rivières",
                province: "Québec",
                codePostal: "J8S 9S6"
            },

        };
    },
};
</script>

<style scoped></style>