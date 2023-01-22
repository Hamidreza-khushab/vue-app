<template>
    <div>
        <h1>{{ name }}</h1>
        <p>{{ i }}</p>
        <p v-if='jender'>man</p>
        <p v-else>woman</p>
        <p class="customer" v-for="customer in customers" :key="customer.id">{{ customer.name }} , {{ customer.city }}</p>
    </div>
</template>

<script>
export default {
    name: 'HeaderApp',
    components: {},
    data: () => ({
        name: 'Hello Saeed!',
        i: 1,
        jender: true,
        customers: [
            { id: 1, name: 'saeed', city: 'Breman' },
            { id: 2, name: 'behnam', city: 'chemnitz' }
        ]
    })
}

</script>

<style scoped>
.customer{
    color: red;
}
</style>