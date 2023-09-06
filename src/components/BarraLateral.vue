<template>
    <header>
        <h1>
            <img src="../assets/logo.png" alt="">
        </h1>
    </header>
</template>

<script lang="ts">
import { difeneComponent } from 'vue'

export default difeneComponent({
    name: 'BarraLateral'
})
</script>

<style scoped>
/* todo o estilo do componenete */
header {
    background: #0d3b66;
    width: 100%;
    height: 100vh;
}
</style>