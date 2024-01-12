<template>
  <footer>
    <div class="relative max-w-[1380px] mx-auto mt-24 py-24 border-t border-white/20">
      <div class="text-white text-center mb-10">
        <h3 class="text-xl font-bold">
          LaraNuxtStore.com
        </h3>
      </div>
      <div class="flex items-center justify-center space-x-4">
        <a
          v-for="(icon, index) in socialIcons"
          :key="index"
          class="bg-white rounded-full p-1"
          >
          <Icon
            :name="icon"
            size="30"
            />
        </a>
      </div>
    </div>
    <div class="flex items-center justify-center bg-primary text-white border-t border-[#262361] py-6">
      <p class="text-sm text-white/30">
        &copy; {{ currentYear }} thandevstrike. All Rights Reserved.
      </p>
    </div>
  </footer>
</template>
<script setup lang="ts">
const socialIcons: string[] = [
  'mdi:facebook',
  'mdi:instagram',
  'mdi:linkedin',
  'mdi:google-plus'
]

const currentYear = computed(() => new Date().getFullYear())
</script>
