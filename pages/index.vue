<template>
  <div>
    <div class="relative w-full h-[600px] bg-hero-banner bg-cover bg-no-repeat bg-bottom rounded">
      <div class="relative flex items-center w-full h-full max-w-5xl text-white mx-auto">
        <div class="w-1/2">
          <div class="relative mb-10">
            <h1 class="text-5xl font-extrabold">
              Perfect
              <GradientText>
                Furniture
              </GradientText>
              for Your
              <GradientText>
                Space
              </GradientText>
            </h1>
          </div>
          <div class="relative mb-10">
            <p>
              Explore a curated collection of home furniture designed to enhance your living space.
            </p>
          </div>
          <div>
            <AppButton>
              Shop now
            </AppButton>
          </div>
        </div>
        <div class="w-1/2" />
      </div>
    </div>
    <div class="flex items-center justify-around flex-wrap text-white/25 py-12">
      <div
        v-for="(partner, index) in partners"
        :key="index"
        >
        <h1 class="text-2xl font-extrabold">
          {{ partner }}
        </h1>
      </div>
    </div>
    <div class="relative py-12">
      <div class="text-white text-center mb-12">
        <h2 class="mb-3">
          Upscale Living
          <GradientText>
            Collection
          </GradientText>
        </h2>
        <span>
          Distinctive Elegance: Unveiling the Exclusive Furniture Collection
        </span>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
        <div
          v-for="(furniture, index) in featureFurnitures"
          :key="index"
          class="relative text-white text-center"
          >
          <div class="relative mb-8">
            <img
              :src="furniture.image"
              class="w-full h-96 rounded"
              >
          </div>
          <div>
            <h3 class="text-xl font-bold">
              {{ furniture.label }}
            </h3>
          </div>
        </div>
      </div>
    </div>
    <div class="relative py-12">
      <div class="text-white text-center mb-12">
        <h2 class="mb-3">
          <GradientText>
            Tailored  Features
          </GradientText>
          Just for You
        </h2>
        <span>
          Distinctive Elegance: Unveiling the Exclusive Furniture Collection
        </span>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
        <div
          v-for="(feature, index) in specialFeatures"
          :key="index"
          >
          <div class="bg-primary text-white w-full h-52 border border-[#262361] rounded p-4">
            <div class="relative mb-6">
              <Icon
                :name="feature.icon"
                color="white"
                size="34"
                />
            </div>
            <div class="relative mb-4">
              <h3 class="text-xl font-bold">
                {{ feature.label }}
              </h3>
            </div>
            <div>
              <p>
                {{ feature.description }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="relative py-12">
      <div class="flex items-center flex-col lg:flex-row py-12">
        <div class="w-full lg:w-1/2">
          <div class="w-full h-[500px]">
            <img
              src="/images/modern-chair.jpg"
              class="w-full h-full rounded"
              >
          </div>
        </div>
        <div class="w-full lg:w-1/2 pl-0 lg:pl-24">
          <div class="text-white mb-12">
            <h2 class="mb-3">
              Our chairs marry
              <GradientText>
                modern style
              </GradientText>
              with
              <GradientText>
                timeless elegance.
              </GradientText>
            </h2>
            <span>
              Distinctive Elegance: Unveiling the Exclusive Furniture Collection
            </span>
          </div>
          <AppButton transparent>
            Read More
          </AppButton>
        </div>
      </div>
      <div class="flex items-center flex-col lg:flex-row py-12">
        <div class="w-full lg:w-1/2 pr-0 lg:pr-24 order-last lg:order-first">
          <div class="text-white mb-12">
            <h2 class="mb-3">
              Explore over
              <GradientText>
                10,000 captivating products
              </GradientText>
              in our collection.
            </h2>
            <span>
              Distinctive Elegance: Unveiling the Exclusive Furniture Collection
            </span>
          </div>
          <AppButton transparent>
            Read More
          </AppButton>
        </div>
        <div class="w-full lg:w-1/2">
          <div class="w-full h-[500px]">
            <img
              src="/images/10k-collections.jpg"
              class="w-full h-full rounded"
              >
          </div>
        </div>
      </div>
      <div class="flex items-center flex-col lg:flex-row py-12">
        <div class="w-full lg:w-1/2">
          <div class="w-full h-[500px]">
            <img
              src="/images/stylish-room.jpg"
              class="w-full h-full rounded"
              >
          </div>
        </div>
        <div class="w-full lg:w-1/2 px-0 lg:px-24">
          <div class="text-white mb-12">
            <h2 class="mb-3">
              Enhance your room with a diverse array of
              <GradientText>
                stylish accessories.
              </GradientText>
            </h2>
            <span>
              Distinctive Elegance: Unveiling the Exclusive Furniture Collection
            </span>
          </div>
          <AppButton transparent>
            Read More
          </AppButton>
        </div>
      </div>
      <div class="flex items-center flex-col lg:flex-row py-12">
        <div class="w-full lg:w-1/2 pr-0 lg:pr-24 order-last lg:order-first">
          <div class="text-white mb-12">
            <h2 class="mb-3">
              We offer
              <GradientText>
                top-tier quality products
              </GradientText>
              in the market.
            </h2>
            <span>
              Distinctive Elegance: Unveiling the Exclusive Furniture Collection
            </span>
          </div>
          <AppButton transparent>
            Read More
          </AppButton>
        </div>
        <div class="w-full lg:w-1/2">
          <div class="w-full h-[500px]">
            <img
              src="/images/quality-products.jpg"
              class="w-full h-full rounded"
              >
          </div>
        </div>
      </div>
    </div>
    <div class="relative py-12">
      <div class="text-white text-center mb-12">
        <h2 class="mb-3">
          Our
          <GradientText>
            Popular Product
          </GradientText>
        </h2>
      </div>
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-12">
        <div
          v-for="n in 4"
          :key="n"
          >
          <div class="bg-gray-700 w-full h-96">
            <img
              src="/images/product_--1.jpg"
              class="w-full h-full rounded"
              >
          </div>
        </div>
      </div>
      <div class="flex justify-center mt-16">
        <AppButton>
          See all product
        </AppButton>
      </div>
    </div>
  </div>
</template>
<script setup lang="ts">
definePageMeta({
  layout: 'landing'
})

const featureFurnitures: { label: string, image: string }[] = [
  {
    label: 'Living Room',
    image: '/images/living-room.jpg'
  },
  {
    label: 'Bedroom',
    image: '/images/bedroom.jpg'
  },
  {
    label: 'Workspace',
    image: '/images/workspace.jpg'
  },
  {
    label: 'Kitchen',
    image: '/images/kitchen.jpg'
  }
]

const specialFeatures = [
  {
    label: 'Easy Payment',
    description: 'Seamless Transactions, Stress-Free Payments',
    icon: 'mdi:credit-card'
  },
  {
    label: 'Lots of Promos',
    description: 'Unlock a treasure trove of exciting deals and discounts.',
    icon: 'mdi:trophy-award'
  },
  {
    label: 'Fast Shipping',
    description: 'Get it quick with our express shipping service.',
    icon: 'mdi:truck-delivery'
  },
  {
    label: 'Save in Cart',
    description: 'Your personal shopping vault – Save in Cart and savor later.',
    icon: 'mdi:cart'
  }
]

const partners: string[] = [
  'Houbi',
  'Fast Company',
  'Duo-Fast',
  'Hornet',
  'Chase'
]
</script>
