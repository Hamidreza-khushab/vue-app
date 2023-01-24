<template>
    <div>
        <div class="menuh">
            <p v-for="menu in menus" :key="menu">{{ menu }} </p>
        </div>
        <h1>{{ title }}</h1>
        <h2 v-if="extD">{{ titleD }}</h2>
        <h2>{{ name }}</h2>
        <p>{{ i }}</p>
        <p v-if='jender'>man</p>
        <p v-else>woman</p>
        <p class="customer" v-for="customer in customers" :key="customer.id">{{ customer.name + '   ' + customer.city}} </p>
    </div>
</template>

<script>
export default {
    name: 'HeaderApp',
    props: {
    title: String,
    titleD: String,
    extD : Boolean,
    menus : Array
  },
    components: {},
    data: () => ({
        name: 'Hello Saeed!',
        i: 1,
        jender: true,
        customers: [
            { id: 1, name: 'saeed', city: 'Breman' },
            { id: 2, name: 'behnam', city: 'Chemnitz' }
        ]
    })
}

</script>

<style scoped>
.customer{
    color: red;
}
.menuh{
    display: flex;
    gap: 10px;
}
</style>