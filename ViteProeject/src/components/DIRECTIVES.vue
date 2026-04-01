<template>
    <div>
        <button @click="show = !show">Click me show</button>
        <h1 v-if="show" v-html="mesage"></h1>
        <hr>
        <h2 v-show="show" v-html="mesage"></h2>
    </div>
    <div>
        <input type="text" v-model="mesage">
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    const mesage = ref('FPT Polytechnic')
    const show = ref(true)
</script>

<style lang="scss" scoped>

</style>