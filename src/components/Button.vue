<template>
    <div>
        <p> Quantity: {{value}} </p>
        <button v-on:click="increment"> + </button>
        <button v-on:click="decrement"> - </button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            value: 0
        }
    },

    methods: {
        increment: function() {
            return this.value = this.value + 1;
        },

        decrement: function() {
            return this.value = this.value - 1;
        }
    }
}
</script>

<style scoped>
    button {
        font-family: 'Avenir', Arial, Helvetica, sans-serif;
        text-align: center;
        color: black;
        font-weight: bold;

    }
</style>