<template>
  <div class="bg-white py-24 sm:py-32">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl text-center">
        <h2 class="text-3xl font-bold tracking-tight text-gray-900 sm:text-4xl">Camper's Guide Sections</h2>
        <p class="mt-2 text-lg leading-8 text-gray-400">Click to Jump</p>
      </div>
      <div class="mx-auto mt-16 grid max-w-2xl auto-rows-fr grid-cols-1 gap-8 sm:mt-20 lg:mx-0 lg:max-w-none lg:grid-cols-3">
        <article v-for="post in posts" :key="post.id" class="relative isolate flex flex-col justify-end overflow-hidden rounded-2xl bg-gray-900 px-8 pb-8 pt-80 sm:pt-48 lg:pt-80">
          <img :src="post.imageUrl" alt="" class="absolute inset-0 -z-10 h-full w-full object-cover" />
          <div class="absolute inset-0 -z-10 bg-gradient-to-t from-gray-900 via-gray-900/40" />
          <div class="absolute inset-0 -z-10 rounded-2xl ring-1 ring-inset ring-gray-900/10" />
          <h3 class="mt-3 text-lg font-semibold leading-6 text-white">
            <a :href="post.href">
              <span class="absolute inset-0" />
              {{ post.title }}
            </a>
          </h3>
        </article>
      </div>
    </div>
  </div>
</template>

<script setup>
import camping_1 from '@/assets/camping_1.webp'
  const posts = [
    {
      id: 1,
      title: 'General Information, Fees, and Parking',
      href: '#general-information',
      imageUrl:
        camping_1,
    },
    {
      id: 2,
      title: 'TRC Standing Rules',
      href: '#rules',
      imageUrl:
        camping_1,
    },
    {
      id: 3,
      title: 'Photography and Video Recording',
      href: '#photography',
      imageUrl:
        camping_1,
    },
    {
      id: 4,
      title: 'Campground Maintenance and Wildlife Habitat Enhancement',
      href: '#campground',
      imageUrl:
        camping_1,
    },
    {
      id: 5,
      title: 'Rules Violations and Dispute Resolution',
      href: '#violations',
      imageUrl:
        camping_1,
    },
    {
      id: 6,
      title: 'General Steps of Consequence',
      href: '#consequence',
      imageUrl:
        camping_1,
    },
    {
      id: 7,
      title: 'Seasonal Camping at TRC',
      href: '#seasonal-camping',
      imageUrl:
        camping_1,
    },
    {
      id: 8,
      title: 'Bylaws',
      href: '#bylaws',
      imageUrl:
        camping_1,
    },
  ]
  </script>