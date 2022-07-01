<template>
    <div>
        <h1>Home</h1>
        <h1>{{count}}</h1>
        <button @click="addCount">+1</button>
    </div>

</template>

<style scoped>
h1{
    text-align: center;
    color: blue;
}
</style>

<script>
export default {
    computed: {
        count() {
            return this.$store.getters.count
        }
    },
    methods: {
        addCount() {
            this.$store.commit("addCount",1)
        }
    }
}
</script>