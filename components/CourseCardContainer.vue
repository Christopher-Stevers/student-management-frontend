<script setup>
const { data }=await useFetch('/api/courses');
let courseData= data._rawValue.data;
console.log(courseData);
let courseJSON=JSON.stringify(courseData);
</script>

<template>
<ul>
    
    <CourseCard v-for="item in courseData" :key="item" :item="item" />
        


</ul>
</template>


<style scoped>
</style>