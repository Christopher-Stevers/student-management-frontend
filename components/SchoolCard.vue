<script setup>
const props = defineProps({
  item: Object,
});
console.log(props.item);
</script>

<template>
<li>
    <p>
{{props.item.title}}</p>
<p>
Address: {{props.item.streetAddress}}</p>
<p>
City: {{props.item.cityAddress}}</p>
<p>
email: {{props.item.email}}</p>




</li>
</template>


<style scoped>
</style>