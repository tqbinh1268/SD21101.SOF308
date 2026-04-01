<template>
    <div>
        <div v-for="(post, index) in props.posts" :key="index">
            <h2>{{ post.title }}</h2>
            <p>{{ post.content }}</p>
            <p>Author: {{ post.author }}</p>
        </div>
    </div>
</template>

<script setup>
    const props = defineProps({
        posts: {
            type: Array,
            required: true,
        } 
    });
</script>

<style lang="scss" scoped>

</style>