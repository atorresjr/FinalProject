<template>
  <div
    class="mt-8 border-double border-4 border-yellow-200 rounded-md container mx-auto w-auto h-screen bg-green-600"
  >
    <div class="grid gap-4 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 mt-4 container mx-auto">
      <keyboard v-for="n in 10" :key="n" />
      <InventoryAdd />
    </div>
  </div>
  <AddForm v-if="show" />
</template>

<script setup>
import { onMounted } from 'vue'
import { show, notes, getAll } from '~/helpers/useForm'
onMounted(() => refresh())
const refresh = async () => await getAll()
</script>

