<template>
    <svg width="32" height="32" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M6 7H16" stroke="white" stroke-opacity="0.7" stroke-width="4" stroke-linecap="round" />
        <path d="M6 16H26" stroke="white" stroke-opacity="0.7" stroke-width="4" stroke-linecap="round" />
        <path d="M16 25L26 25" stroke="white" stroke-opacity="0.7" stroke-width="4" stroke-linecap="round" />
    </svg>
</template>

<script setup lang="ts">
 const props = defineProps<{
    class?: string
 }>()
</script>