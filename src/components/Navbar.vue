<template>
    <div class="container">
        <Hamburger />
    </div>
</template>

<script lang="ts">
import Hamburger from './Hamburger.vue';


export default {
    components: {
        Hamburger,
    }
}
</script>

<style scoped>
    .container {
        display: flex;
        height: 96px;
        padding: 24px 240px;
        justify-content: center;
        align-items: center;
        gap: 60px;
        align-self: stretch;
    }
</style>