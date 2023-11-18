<template>
  <div>
   
    <img src="../assets/images/image1.svg" loading="lazy" />

   


    <div class="flex items-center gap-5 py-16 px-16 justify-between">
     
      <div
        class="flex flex-col justify-center items-center"
        v-for="category in categories"
        :key="category.name"
      >
      
        <img
          class="rounded-full w-44"
          :src="category.img"
          alt=""
          loading="lazy"
        />
        <span class="text-lg font-semibold">{{ category.name }}</span>
      </div>
    </div>

    <div>
      <div class="flex items-center justify-between gap-4 px-16">
        <div class="w-1/2">
          <img loading="lazy" src="../assets/images/image2.svg" />
        </div>
        <div class="w-1/2">
          <img loading="lazy" src="../assets/images/image3.svg" />
        </div>
      </div>

      <div class="flex items-center justify-between gap-4 px-16 py-4">
        <div class="w-1/3">
          <img loading="lazy" src="../assets/images/image4.svg" />
        </div>
        <div class="w-1/3">
          <img loading="lazy" src="../assets/images/image5.svg" />
        </div>
        <div class="w-1/3">
          <img loading="lazy" src="../assets/images/image6.svg" />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import group244 from '@/assets/images/Group244.png'
import group245 from '@/assets/images/Group245.png'
import group246 from '@/assets/images/Group246.png'
import group247 from '@/assets/images/Group247.png'
import group248 from '@/assets/images/Group248.png'
import group249 from '@/assets/images/Group249.png'

const image = '../assets/images'
const categories = [
  {
    name: "Men's T-Shirts",
    img: group244,
  },
  {
    name: "Women's Wear",
    img: group245,
  },
  {
    name: 'Winter Collections',
    img: group246,
  },
  {
    name: 'Hooded T-Shirts',
    img: group247,
  },
  {
    name: 'Polo Neek T-Shirts',
    img: group248,
  },
  {
    name: 'Full Sleeves T-Shirts',
    img: group249,
  },
]
</script>
