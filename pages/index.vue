<template>
    <div>
        <h1>hello Nuxt</h1>
        <h2>{{ name }}</h2>
        <h2>{{ age }}</h2>
    </div>
</template>

<script>
export default {
    name: "index",
    asyncData(context) {
        console.log(context);
        console.log(process.server);
        return { name: "zhangsan" };
    },
    data() {
        return {
            age: 18,
        };
    },
};
</script>

<style>
</style>