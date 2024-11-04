<template>
    <div>
        <div v-for="(hobby, index) in hobbies" class="hobby">
            <span>{{ hobby }}</span>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            hobbies: ["sport", "lecture"],

        };
    },
};
</script>

<style scoped>
.hobby {
    display: flex;
    justify-content: space-between;
    padding: 10px;
    margin: 10px auto;
    border-radius: 10px;
    background-color: #f5f5dc;
    color: black;
}
</style>