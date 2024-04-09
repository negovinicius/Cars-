<script>
    import {RouterLink} from "vue-router"
</script>

<template>
    <div>
        <RouterLink active-class="active" to = "/">Home</RouterLink>
        <RouterLink active-class="active" to = "/About">About</RouterLink>
    </div>
</template>

<style scoped>
    .active {
        font-weight: 900;
        color: rgb(156, 103, 5);
    }
</style>