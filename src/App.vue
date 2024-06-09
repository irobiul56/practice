<script setup>

import { ref } from 'vue';

const location = ref('Dhaka')

function changelocation(newlocation){
  location.value = newlocation
}

</script>

<template>
    <div>
        <button @click="changelocation('Dhaka')">Dhaka</button>
        <button @click="changelocation('Rangpur')">Rangpur</button>
        <button @click="changelocation('Khulna')">Khulna</button><br><br>
        <p>Your Location is: {{ location }} </p>
    </div>
</template>
    
<style scoped>

</style>
