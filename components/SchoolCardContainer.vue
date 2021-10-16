<script setup>
const { data }=await useFetch('/api/schools');
let schoolData= data._rawValue.data;
console.log(schoolData);
let schoolJSON=JSON.stringify(schoolData);
</script>

<template>
<ul>
    
    <SchoolCard v-for="item in schoolData" :key="item" :item="item" />
        


</ul>
</template>


<style scoped>
</style>