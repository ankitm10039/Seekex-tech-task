<template>
  <div class="font-sans">
    <AppHeader />
    <HeroSection />

    <ProductSection title="Trending T-Shirts" :products="products" />
    <ProductSection title="Featured Products" :products="newProducts" />
    <img src="../assets/images/banner12.svg" loading="lazy" />
    <ProductSection title="New Products" :products="newProducts" />
    <ProductSection title="Best Selling Products" :products="newProducts" />
    <NewProductSec  :newProducts1="newProducts1" />
    <AppFooter />
  </div>
</template>

<script setup>
import AppHeader from '@/components/AppHeader.vue'
import HeroSection from '@/components/HeroSection.vue'
import ProductSection from '@/components/ProductSection.vue'
import AppFooter from '@/components/AppFooter.vue'
import NewProductSec from '@/components/NewProductSec.vue'
import { products, newProducts,newProducts1 } from '@/data/products'
</script>
