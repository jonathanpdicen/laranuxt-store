<template>
  <header>
    <div class="relative max-w-[1380px] mx-auto py-8">
      <div class="w-full flex flex-wrap items-center justify-center md:justify-normal text-white gap-x-16">
        <div class="relative mb-4">
          <h2 class="text-2xl font-bold">
            LaraNuxt Store
          </h2>
        </div>
        <nav class="relative hidden md:block">
          <ul class="flex space-x-8">
            <li
              v-for="(menu, index) in menus"
              :key="index"
              >
              <a href="#">
                {{ menu.name }}
              </a>
            </li>
          </ul>
        </nav>
        <div class="flex items-center space-x-6 ml-0 md:ml-auto">
          <div class="flex space-x-4">
            <Icon
              name="mdi:magnify"
              color="white"
              size="24"
              />
            <Icon
              name="mdi:cart-outline"
              color="white"
              size="24"
              />
          </div>
          <div class="w-[2px] h-4 bg-gray-200" />
          <a
            href="#"
            class="mr-4"
            >
            Sign Up
          </a>
          <AppButton>
            Login
          </AppButton>
        </div>
      </div>
    </div>
  </header>
</template>
<script setup lang="ts">
const menus: { name: string, path?: string }[] = [
  {
    name: 'Home',
    path: ''
  },
  {
    name: 'Products',
    path: ''
  },
  {
    name: 'Newsfeed',
    path: ''
  },
  {
    name: 'Promo',
    path: ''
  },
]
</script>
