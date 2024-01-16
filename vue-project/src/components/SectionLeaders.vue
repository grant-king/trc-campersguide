<template>
  <div class="bg-white py-24 sm:py-32" id="toc">
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
import gen_info from '@/assets/gen_info.webp'
import standing_rules from '@/assets/standing_rules.webp'
import photography from '@/assets/photography.webp'
import violations from '@/assets/violations.webp'
import wildlife from '@/assets/wildlife.webp'
import steps from '@/assets/steps.webp'
import seasonal from '@/assets/seasonal.webp'
  const posts = [
    {
      id: 1,
      title: 'General Information, Fees, and Parking',
      href: '#general-information',
      imageUrl:
        gen_info,
    },
    {
      id: 2,
      title: 'TRC Standing Rules',
      href: '#rules',
      imageUrl:
        standing_rules,
    },
    {
      id: 3,
      title: 'Photography and Video Recording',
      href: '#photography',
      imageUrl:
        photography,
    },
    {
      id: 4,
      title: 'Campground Maintenance and Wildlife Habitat Enhancement',
      href: '#campground',
      imageUrl:
        wildlife,
    },
    {
      id: 5,
      title: 'Rules Violations and Dispute Resolution',
      href: '#violations',
      imageUrl:
        violations,
    },
    {
      id: 6,
      title: 'General Steps of Consequence',
      href: '#consequence',
      imageUrl:
        steps,
    },
    {
      id: 7,
      title: 'Seasonal Camping at TRC',
      href: '#seasonal-camping',
      imageUrl:
        seasonal,
    },
  ]
  </script>