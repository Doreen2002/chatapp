<script setup>
import { ref } from 'vue';

const messages = ref([
    {
        image:"../assets/avatar.jpeg",
        username : "Doreen",
        dateTime: "",
        message: "Text test",
        unread:3

    },
    {
        image:"../assets/avatar.jpeg",
        username : "Doreen",
        dateTime: "",
        message: "Text test",
        unread:3

    },
    {
        image:"../assets/avatar.jpeg",
        username : "Doreen",
        dateTime: "",
        message: "Text test",
        unread:3

    }
])
</script>



<template>
   
    <div class="flex mx-3 my-2 border rounded-t-lg border-pink-100 p-4" v-for="(item, key) in messages" :key="key">
        <div><img :src=item.image class="w-16 h-16 border rounded-full"/></div>
        <div class="flex flex-col flex-grow  ">
            <div class="flex justify-between"><div>{{ item.username }}</div><div>{{ item.dateTime }}</div></div>
            <div class="flex justify-between"><div>{{ item.message }}</div><div>{{ item.unread }}</div></div>
        </div>
    </div>
    
    
</template>