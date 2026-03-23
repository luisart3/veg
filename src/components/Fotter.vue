<script setup lang="ts">
import { ChevronDownIcon  } from '@heroicons/vue/24/outline';

const foods = [
    {
        
        name: 'Sandwich',
        price: 'Rs. 129/-',
        url: '../src/assets/Sandwich.png'
    }, 
    {
        
        name: 'Pizza',
        price: 'Rs. 129/-',
        url: '../src/assets/Pizza.png'
    },
    {
        
        name: 'Biryani',
        price: '',
        url: '../src/assets/Biryani.png'
    },
    {
        
        name: 'Burger',
        price: '',
        url: '../src/assets/Burger.png'
    }
]
</script>

<template>
    <div class="fixed bottom-0 left-0 w-full max-h-[40vh] overflow-y-auto bg-white/5 rounded-t-3xl backdrop-blur-md p-6">
        <div class="grid lg:grid-cols-4 grid-cols-2 gap-10">
            <div v-for="food in foods" :key="food.name" class="flex flex-row items-center gap-5">
                <img :src="food.url" class=" border-transparent rounded-full lg:h-20 lg:w-20 h-14 w-14"/>
                <div class="flex flex-col space-y-1 ">
                    <h3 class="font-medium text-white text-xl">{{ food.name }}</h3>
                    <p class=" font-light text-white text-sm">{{ food.price }}</p>
                    <button type="button" class="flex cursor-pointer px-1.5 py-1.5 gap-2 items-center bg-white/10 hover:bg-white/20 transition rounded-md font-medium text-sm">Click Here <ChevronDownIcon class="size-4"/></button>
                </div>
            </div>
        </div>
        
    </div>
</template>