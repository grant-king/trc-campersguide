<template>
    <footer class="bg-white">
      <div class="mx-auto max-w-7xl overflow-hidden px-6 py-20 sm:py-24 lg:px-8">
        <nav class="-mb-6 columns-2 sm:flex sm:justify-center sm:space-x-12" aria-label="Footer">
          <div v-for="item in navigation.main" :key="item.name" class="pb-6">
            <a :href="item.href" class="text-sm leading-6 text-gray-600 hover:text-gray-900">{{ item.name }}</a>
          </div>
        </nav>
        <p class="mt-10 text-center text-xs leading-5 text-gray-500">This website is a development experiment intended to provide a sample convenice tool. This site <a href="https://trianglehat.org">https://trianglehat.org</a> is not endorsed by or associated with Triangle Recreation Camp.</p>
      </div>
    </footer>
  </template>
  
  <script setup>
  import { defineComponent, h } from 'vue'
  
  const navigation = {
    main: [
      { name: 'Top', href: '#' },
      { name: 'Donate to TRC', href: 'https://camptrc.org/Donate' },
    ]
    }
  </script>
