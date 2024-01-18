<template>
  <div :id="section.id" class="bg-white py-24 md:py-32">
    <div class="mx-auto grid max-w-7xl grid-cols-1 gap-x-8 gap-y-20 px-6 lg:px-8 xl:grid-cols-5">
      <div class="max-w-2xl xl:col-span-2">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">{{ section.title }}</h2>
        <p class="mt-6 text-lg leading-8 text-gray-600">{{ section.description }}</p>
      </div>
      <ul role="list" class="-mt-12 space-y-12 divide-y divide-gray-200 xl:col-span-3">
        <li v-for="part in section.parts" :key="part.id" class="transition-all duration-200 flex flex-col gap-10 pt-12 sm:flex-row" :id="part.href">
          <div @click="toggleContentVisibility(part.id)" class="border-solid border-4 border-black opacity-50 drop-shadow-xl flex-none bg-gradient-to-b from-rose-300 via-green-600 to-violet-900 rounded">
            <img :class="{'ml-auto': isToggled[part.id], 'mr-auto': !isToggled[part.id], 'opacity-60':!isToggled[part.id], 'interactive-image':true, 'aspect-[4/5]':true, 'flex-none':true, 'w-44':true, 'rounded-2xl':true, 'object-cover':true }" :src="part.imageUrl" alt="" />
          </div>
          <div class="max-w-xl flex-auto">
              <h3 class="text-lg font-semibold leading-8 tracking-tight text-gray-900">{{ part.title }}</h3>
              <p class="mt-6 text-base leading-7 text-gray-600">{{ part.description }}</p>
              <div :id="part.id" :class="{'visible': isToggled[part.id], 'hidden':!isToggled[part.id]}">
                <div v-for="content in part.content" :key="content.heading" class="mt-6" >
                  <h4 class="text-base font-semibold leading-6 tracking-wide text-gray-900">{{ content.heading }}</h4>
                  <div v-html="content.body" class="mt-2 leading-6 text-gray-600"></div>
                  <div v-if="content.list">
                    <ul role="list" class="mt-2 leading-6 text-gray-600">
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
import { ref, reactive } from 'vue'
import camping_1 from '@/assets/camping_1.webp'

defineProps({
  section: {
    type: Object,
    required: true
  }
})

const isToggled = ref({})

function toggleContentVisibility(part_id) {
  if (isToggled.value[part_id] === undefined) {
    isToggled.value[part_id] = true;
  }
  else {
    isToggled.value[part_id] = !isToggled.value[part_id];
  }
}

</script>

<style scoped>

.interactive-image {
  cursor: pointer;
}

</style>