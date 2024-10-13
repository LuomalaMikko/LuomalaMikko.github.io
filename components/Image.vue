<template>
    <NuxtLink :to=pageLink>
        <img class="max-h-32 mb-4" :src=imageUrl>
    </NuxtLink>

</template>

<script setup>

const props = defineProps({
    imageUrl: String,
    pageLink: String,
})

</script>

<style lang="scss" scoped>
</style>