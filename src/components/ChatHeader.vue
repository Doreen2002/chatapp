<script setup>
import { Bars3Icon,PlusIcon , MagnifyingGlassIcon} from '@heroicons/vue/24/solid'
</script>


<template>
    <div class="">
        <div class="flex flex-col ">
            <div class="flex justify-between h-10 bg-pink-300 place-items-center px-3 text-white">
                <div><Bars3Icon class="size-6 " /></div>
                <div >Messages </div>
                <div><PlusIcon class="size-6 " /></div>
            </div>
            <div class="flex place-self-center place-items-center my-2 border rounded-md w-96 text-gray-400"><input type="search" placeholder="Search" class="flex-grow  text-center  h-7"/> <MagnifyingGlassIcon class="size-6 "/></div>
        </div>
       
    </div>
</template>