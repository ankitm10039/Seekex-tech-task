<template>
    <div class="px-10 py-16">
      <div class="text-center text-4xl font-medium pb-16">{{ title }}</div>
  
      <div
        class="grid grid-cols-2 lg:grid-cols-3 items-center gap-x-4 gap-y-8 w-full"
      >
        <div
          class="flex flex-col bg-red-40 group"
          v-for="(product, idx) in newProducts1"
          :key="idx"
        >
          <div class="relative w-full overflow-hidden hover:border-100">
            <img class="w-full" :src="product.img" alt="product.title" />
          
            <!-- <div
              class="w-full grid place-items-center opacity-0  h-full top-0 group-hover:backdrop-blur-sm transition-colors absolute z-10"
            >
              
            </div> -->
          </div>
         
        </div>
      </div>
  
    
  
    
    </div>
<div class="border-blue-500">
    <img src="../assets/images/banner13.svg" loading="lazy" />
</div>
   
<!-- 2 images in 2 card -->

    <div class="flex items-center justify-between gap-4 px-16">
        <div class="w-1/1">
          <img loading="lazy" src="../assets/images/image75.svg" />
        </div>
        <div class="w-1/2">
          <img loading="lazy" src="../assets/images/hurryUp.svg" />
        </div>
      </div>

      <!-- new design -->
      <div class="flex  ml-56 items-center justify-between gap-4 px-16 py-4 mt-10">
        <div class="w-1/4">
          <img loading="lazy" src="../assets/images/Group199.png" />
        </div>
        <div class="w-1/4">
          <img loading="lazy" src="../assets/images/Group200.png" />
        </div>
        <div class="w-1/4">
          <img loading="lazy" src="../assets/images/Group201.png" />
        </div>
        <div class="w-1/4">
          <img loading="lazy" src="../assets/images/Group202.png" />
        </div>
      </div>


      <div class="flex  ml-46 items-center justify-between gap-4 px-16 py-10 mt-10">
     

<div class="w-full p-4 text-center bg-red-800 border border-gray-700 rounded-lg shadow sm:p-8 dark:bg-gray-800 dark:border-gray-700">
    <h2 class="mb-2  text-4xl font-bold text-white dark:text-white">Subscribe to get updates on exciting offers
& deals</h2>
 
     <div class="mb-1 text-xs">
 
<form>
    <div class="flex">
        
        <div class="relative w-full  px-6">
            <input type="search" id="search-dropdown" class="block py-6 w-full z-20 text-sm text-gray-900 bg-gray-50 rounded-e-lg rounded-s-gray-100 rounded-s-2 border border-gray-300 focus:ring-blue-500 focus:border-blue-500 dark:bg-gray-700 dark:border-gray-600 dark:placeholder-gray-400 dark:text-white dark:focus:border-blue-500" placeholder="Enter your mail" required>
            <button type="submit" class="absolute top-0 end-0 p-2.5 h-full py-6 text-sm font-medium text-red-900 bg-white rounded-e-lg border border-blue-700  focus:ring-4 focus:outline-none focus:ring-blue-300 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800">
            Subecribe    
            </button>
        </div>
    </div>
</form>

     </div>
</div>

      </div>
  </template>
  
  <script setup>
import { newProducts1 } from '@/data/products';

  defineProps({
    title: String,
    newProducts1: Array,
  })
  </script>
  