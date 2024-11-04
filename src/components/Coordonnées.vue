<template>
    <h3 id="email" @click="modifier()">{{ email }} </h3>
    <h3 id="telephone" @click="modifier()">{{ telephone }}</h3>
    <h3>{{ adresse.numero }} {{ adresse.rue }} <br>
        <span>{{ adresse.ville }}</span> {{ adresse.province }} <br>
        {{ adresse.codePostal }}
    </h3>
</template>

<script>
export default {
    emits: ["modification"],
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
            }
        }
    },
    methods: {
        modifier(e) {
            let id = e.target.id


            switch (id) {
                case 'email':
                    this.email = prompt("Entrer l'email")
                    this.$emit("modification", "Modification de l'email: " + this.email)
                    break;
                case 'telephone':
                    this.telephone = prompt("Entrer le numéro de téléphone")
                    this.$emit("modification", "Modification du téléphone: " + this.telephone)
                    break;
            }
        }
    }
}
</script>

<style scoped></style>