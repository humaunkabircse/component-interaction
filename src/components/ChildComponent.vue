<script setup>
defineProps(['message'])

const emit = defineEmits(['update:message'])

function messageEmitted (){
    emit('update:message', 'I enjoy it so much and found it to be my passion.')
}
</script>

<template>
    <p class="mb-3 text-gray-700 dark:text-gray-400 font-bold">{{ message }}</p>
    <button @click="messageEmitted()" class="inline-flex items-center px-3 py-2 text-sm font-medium text-center text-white bg-blue-700 rounded-lg hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">Click</button>
</template>
<style scoped>

</style>