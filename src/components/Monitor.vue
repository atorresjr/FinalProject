
<template>
    <div class="bg-yellow-400 text-yellow-800 rounded text-center p-2 space-y-2">
        <h3 class="text-2xl font-thin tracking-wide">Monitor Brand</h3>
        <p class="text-sm font-medium text-yellow-900">Monitor Model Will Go Here</p>
        <div class="flex justify-end space-x-5">
            <button class="hover:text-green-800">
                <flat-color-icons:add-database />
            </button>
            <button class="hover:text-red-800">
                <flat-color-icons:full-trash />
            </button>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue'


defineProps({
    default: {
        id: 0,
        title: '',
        content: '',
    },
})

</script>