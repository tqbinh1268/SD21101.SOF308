<template>
    <div>
        <h1>Caculator</h1>
        <div>
            <button style="font-size: 2rem;" @click="increment">+</button>
            <button style="font-size: 2rem;" @click="decrement">-</button>
            <button style="font-size: 2rem;" @click="reset">Reset</button>
        </div>
        <p class="mt-5" style="font-size: 2rem;">Count is {{ count }}</p>
    </div>
</template>

<script setup>
    import { ref } from 'vue'
    const count = ref(0)
    const increment = () => count.value++
    const decrement = () => count.value--
    const reset = () => (count.value = 0)
</script>

<style lang="scss" scoped>

</style>