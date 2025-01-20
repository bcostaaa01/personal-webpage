<template>
    <article
        class="overflow-hidden rounded-lg shadow transition hover:shadow-lg mt-16 bg-gray-100">
        <div class="flex flex-col lg:flex-row">
            <div class="w-1/2" v-if="imageSrc">
                <img :alt="imageAlt" :src="imageSrc" class="h-56 w-56 rounded-full object-cover mx-10 mt-28" />
            </div>
            <div class="ml-10 p-4">
                <h1 class="mt-4 text-3xl text-gray-900 mb-4">{{ title }}</h1>
                <time :datetime="date" class="block text-md text-gray-500">{{ formattedDate }}</time>
                <slot />
            </div>
        </div>
    </article>
</template>

<script setup lang="ts">
defineProps({
    title: String,
    date: String,
    formattedDate: String,
    content: String,
    imageSrc: String,
    imageAlt: String,
});
</script>
