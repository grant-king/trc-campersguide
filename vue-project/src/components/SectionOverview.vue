<template>
  <div :id="section.id" class="bg-white py-24 md:py-32">
    <div class="mx-auto grid max-w-7xl grid-cols-1 gap-x-8 gap-y-20 px-6 lg:px-8 xl:grid-cols-5">
      <div class="max-w-2xl xl:col-span-2">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">{{ section.title }}</h2>
        <p class="mt-6 text-lg leading-8 text-gray-600">{{ section.description }}</p>
      </div>
      <ul role="list" class="-mt-12 space-y-12 divide-y divide-gray-200 xl:col-span-3">
        <li v-for="part in section.parts" :key="part.href" class="flex flex-col gap-10 pt-12 sm:flex-row">
          <img @click="toggleContentVisibility(part.id)" class="interactive-image aspect-[4/5] flex-none w-52 rounded-2xl object-cover" :src="part.imageUrl" alt="" />
          <div class="max-w-xl flex-auto">
              <h3 class="text-lg font-semibold leading-8 tracking-tight text-gray-900">{{ part.title }}</h3>
              <p class="mt-6 text-base leading-7 text-gray-600">{{ part.description }}</p>
              <div :id="part.id" style="display: none;">
                <div v-for="content in part.content" :key="content.heading" class="mt-6" >
                  <h4 class="text-base font-semibold leading-6 tracking-wide text-gray-900">{{ content.heading }}</h4>
                  <div v-html="content.body" class="mt-2 text-sm leading-6 text-gray-600"></div>
                  <div v-if="content.list">
                    <ul role="list" class="mt-2 text-sm leading-6 text-gray-600">
                      <li v-for="item in content.list" :key="item" class="mt-4">{{ item }}</li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
        </li>
      </ul>
    </div>
  </div>
</template>
  
<script setup>

import camping_1 from '@/assets/camping_1.webp'

defineProps({
  section: {
    type: Object,
    required: true
  }
})

function toggleContentVisibility(part_id) {
  const content = document.getElementById(part_id);
  if (content.style.display === "none") {
    content.style.display = "block";
  } else {
    content.style.display = "none";
  }
}

</script>

<style scoped>

.interactive-image {
  cursor: pointer;
}

</style>