<script setup lang="ts">
import { ShoppingBagIcon } from '@heroicons/vue/24/outline';
import IconMenu from './icons/IconMenu.vue';
</script>
<template>
    <nav class=" top-0 left-0 w-full z-20 ">
            <div class=" flex justify-between items-center h-16">
                <div class="hidden lg:flex justify-center items-center gap-14">
                    <a href="#" class=" hover:text-white transition text-white/75  ">Home</a>
                    <a href="#" class="hover:text-white transition text-white/75">Order</a>
                    <a href="#" class="hover:text-white transition text-white/75">Contact Us</a>
                </div>
                <div class="flex justify-center items-center">
                    <a>
                        <img src="/veg.svg" class="h-26"/>
                    </a>
                </div>
                <div class="flex justify-end items-center gap-7">
                    <div class="relative">
                        <ShoppingBagIcon class="size-6"/>
                        <div class="absolute top-0 right-0 translate-x-1/2 -translate-y-1/2 w-2 h-2 bg-lime-500 rounded-full"></div>
                    </div>
                    <div class="flex items-center gap-7">
                        <span>Menu</span>
                        <IconMenu class=" size-6"/>
                    </div>

                </div>

            </div>
    </nav>
</template>