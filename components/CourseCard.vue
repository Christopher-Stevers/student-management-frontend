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
{{props.item.description}}</p>


</li>
</template>


<style scoped>
</style>