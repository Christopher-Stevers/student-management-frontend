<script setup>
import { ref } from 'vue'
const links=ref([
{label: "Home", route: "/"},
{label: "About", route: "/about"},
{label: "Our Schools", route: "/schools" },
{label: "Login", route: "/login"},
{label: "Courses", route: "/courses"}


]);
</script>

<template>
<nav>
    <ul class="list">

        <li v-for="item in links" :key="item">
            
            <nuxt-link :to="item.route">{{item.route}}</nuxt-link>
        </li>

</ul>
</nav>
</template>


<style scoped>
</style>