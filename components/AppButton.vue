<template>
  <button
    class="bg-gradient-to-r from-blue-500 to-green-300 text-white font-semibold rounded p-[2px]"
    :class="{ 'px-6 py-2 text-center border border-white/35 rounded-sm hover:bg-gradient-to-r hover:from-black hover:to-black' : !transparent }"
    :type="type"
    >
    <span
      v-if="transparent"
      class="flex w-full bg-gray-900 text-white rounded py-3 px-6"
      >
      <slot />
    </span>
    <template v-else>
      <slot />
    </template>
  </button>
</template>
<script setup lang="ts">
defineProps({
  type: {
    type: String as () => 'submit' | 'button',
    default: () => 'submit',
  },
  transparent: {
    type: Boolean,
    default: () => false,
  },
  full: {
    type: Boolean,
    default: () => false,
  }
})
</script>
