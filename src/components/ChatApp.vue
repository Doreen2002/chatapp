<script setup>
import ChatHeader from './ChatHeader.vue';
import MessageList from './MessageList.vue';
</script>

<template>
    <div class="max-w-3xl">
        <ChatHeader/>
        <div class="border h-dvh border-gray-200 py-3 mx-2 rounded-t-lg">
            <MessageList/>
        </div>
        
        

    </div>
   
</template>