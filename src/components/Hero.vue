<script setup lang="ts">
import { MapPinIcon, MagnifyingGlassIcon, ChevronDownIcon, PlusIcon } from '@heroicons/vue/24/outline';
import { StarIcon } from '@heroicons/vue/24/solid';
</script>

<template>
    <section class="absolute  md:inset-y-0 inset-y-26 flex md:items-center">
        <div class=" max-w-lg">
            <div class="flex flex-col space-y-5 ">
                <h2 class="lg:text-7xl text-6xl font-semibold text-white/75 tracking-tight leading-tight">Healthy Veg
                    Outlet
                </h2>
                <div class=" max-w-xs flex-col space-y-5">
                    <div class="flex justify-between items-center border-2 rounded-full px-1 py-1 space-x-3  w-full">
                        <button
                            class="flex items-center gap-3.5 px-2.5 cursor-pointer transition hover:bg-[#557d33] py-2 border-radius bg-[#66913E]/90 backdrop-blur-sm">
                            <MapPinIcon class="size-6" />
                            Location
                            <ChevronDownIcon class="size-4" />
                        </button>
                        <div class="relative ">
                            <input id="search" type="serach" name="search" placeholder="Search"
                                class="block outline-none rounded-full px-3 w-full py-2 focus:ring-2 focus:ring-[#C97303]/50" />
                            <button
                                class="absolute top-1/2 right-1 -translate-y-1/2 bg-[#C97303] px-2 py-2 rounded-full hover:bg-[#975209] transition cursor-pointer">
                                <MagnifyingGlassIcon class="size-6" />
                            </button>
                        </div>

                    </div>
                    <div class="flex items-center space-x-2.5  bg-white/5 rounded-full backdrop-blur-xs p-3 border border-white/10">
                        <div class="flex items-center gap-1">
                            <h3 class="font-medium text-xl">1M </h3>
                            <PlusIcon class="size-4 stroke-3" />
                        </div>
                        <div class="flex space-x-1.5 items-center">
                            <div class="flex">
                                <div v-for="n in 5" :key="n">
                                    <StarIcon :class="{'size-4': n >=1, '[mask-image:linear-gradient(to_right,black,transparent)]': n===5}" />
                                </div>
                            </div>
                            <h3 class="font-medium text-lg">4.5 Star Rating</h3>
                        </div>

                    </div>
                </div>
            </div>
        </div>

        
        <div class=" fixed right-8 top-1/3">
            <div class="md:flex space-y-11 flex-col hidden">
                <div v-for="n in 4" :key="n">
                    <div :class="{ 'bg-white w-5 h-5 rounded-full': n === 1, 'bg-white h-3 w-3 rounded-full': n >= 2 }">
                    </div>
                </div>
            </div>
        </div>




    </section>
</template>
