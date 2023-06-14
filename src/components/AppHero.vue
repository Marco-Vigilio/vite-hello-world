<script>
import AppTitle from "./AppTitle.vue";
export default {
    components: {
        AppTitle,
    },
    data() {
        return {
            jumbo: "JUMBO",
            tron: "TRON",
            contatore: 0,
        }
    },
    methods: {
        incrementaContatore() {
            this.contatore++
        }
    }
}
</script>

<template>
    <div>
        <span class="blue">{{ jumbo }}</span><span class="yellow">{{ tron }}</span>
        <AppTitle />
        <p>Contatore {{ contatore }}</p>
        <button @click="incrementaContatore">Click</button>
    </div>
</template>

<style>
div {
    font-family: Arial, Helvetica, sans-serif;
    text-align: center;
    padding: 1rem;
    background-color: rgb(238, 221, 255);
}

span {
    font-size: 4rem;
}

.yellow {
    color: rgb(255, 180, 29);
}

.blue {
    color: rgba(0, 0, 131, 0.747);
}

button {
    padding: .5rem;
}
</style>
