<template>
    <h1>ホーム！！！</h1>
    <input v-model="text">
    <h3>{{ text }}</h3>
</template>

<script setup lang="ts">
import { ref } from 'vue';
import { useHead } from 'unhead';
import { headData } from './ts/head';

useHead({
    title: headData.home.title
});

const text = ref('')

</script>