<template>
    <h1 class="text-[30px] font-bold sm:text-[50px] text-center">
        {{ props.title }}
    </h1>
</template>

<script setup>
 const props = defineProps({
    title:String
 })
</script>
