<script setup>

import { defineProps} from 'vue';
defineProps(['title'])


</script>



<template>
<h2>{{ title }}</h2>
<button @click="$emit('enlarge-text')">Enlarge Text</button>
</template>
