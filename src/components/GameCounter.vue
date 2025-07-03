<script setup>
console.log('componente de juego')
const isActive = true
</script>

<template>
    <button>menos</button>
    <span class="counter" :class="{ 'counter--active': isActive }">contador: <span>0</span></span>
    <button>más</button>
</template>

<style scoped lang="scss">
.counter {
    font-weight: bold;
    font-size: 2.5rem;

    &>span {
        color: green;
    }
}

.counter--active {
    background-color: #ddd;
}

.counter--active button {
    background-color: red;
}
</style>