<script setup>
import {ref, reactive} from 'vue';
import ChildComponent from './ChildComponent.vue';

const person = reactive({
    name: 'HUMAUN KABIR',
    age: 33,
    occupation: 'Web Developer',
    message: 'Why I love being a web developer ?',
});

</script>

<template>
<div class="max-w-sm p-6 bg-white border border-gray-200 rounded-lg shadow dark:bg-gray-800 dark:border-gray-700">
    <h2 class="mb-2 text-xl tracking-tight text-gray-900 dark:text-white">Name: {{ person.name }}</h2>
    <h2 class="mb-2 text-xl tracking-tight text-gray-900 dark:text-white">Age: {{ person.age }}</h2>
    <h2 class="mb-2 text-xl tracking-tight text-gray-900 dark:text-white">Occupation: {{ person.occupation }}</h2>
    <ChildComponent v-model:message="person.message" />
</div>


</template>
<style scoped>

</style>