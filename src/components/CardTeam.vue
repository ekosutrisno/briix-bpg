<template>
    <div class="lg:min-w-[200px] lg:max-w-[200px] group pb-2 transition">
        <div class="lg:h-[200px] bg-[#D9D9D9] overflow-hidden rounded-xl">
            <img 
                class="w-full h-full object-cover" 
                :src="team.img ? team.img : 'https://t4.ftcdn.net/jpg/02/17/34/67/240_F_217346782_7XpCTt8bLNJqvVAaDZJwvZjm0epQmj6j.jpg'" 
                :alt="team.name"
            >
        </div>
        <div class="mt-2 font-manrope">
            <p class="text-xl font-normal text-briix-primary">{{ team.name }}</p>
            <p class="font-ligh mt-2">{{ team.title }}</p>
        </div>
        <div class="h-0.5 w-1/2 rounded-md group-hover:bg-briix-primary mt-2"></div>
    </div>
</template>

<script setup lang="ts">
defineProps<{team: {
    img: string,
    name: string,
    title: string
}}>()

</script>

<style scoped>

</style>