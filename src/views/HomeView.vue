<script setup> 
    import cars from "../data/cars.json"
    import {RouterLink} from "vue-router"
</script>

<template>
    <div>
        <h1>Home View</h1>
        <div class="cars">
            <RouterLink :to="`/cars/${car.id}`" v-for="car in cars" :key="car.id">
            {{ car.name }}
        </RouterLink>
        </div>
    </div>

<br>    

<h2>In construction..</h2>

</template>

<style scoped>
    .cars {
        display: flex;
    }
    .cars a {
        text-decoration: none;
        color: rgb(153, 5, 143);
        width: 100%;
        box-shadow: 1px 1px 1px 1px;
        margin: 10px;
    }
</style>



