<script setup>

const emit = defineEmits(['sort-by'])
</script>

<template>
  <span class="mr-3 font-bold rounded-l">Order by:</span>
  <div class="inline-flex mb-8">
    <button
      class="bg-gray-300 hover:bg-gray-400 text-gray-800 font-bold py-2 px-3 rounded-l"
      @click="emit('sort-by', 'id')"
    >
    1-9
      <!-- <IconOrderNumber /> -->
    </button>
    <button
      class="border-l border-gray-500 bg-gray-300 hover:bg-gray-400 text-gray-800 font-bold py-2 px-3 rounded-r"
      @click="emit('sort-by', 'name')"
    >
    A-Z
      <!-- <IconOrderAlpha /> -->
    </button>
  </div>
</template>
