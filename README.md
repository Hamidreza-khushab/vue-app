# vue_treaning

## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).


``` 
<h1>{{ name }}</h1>
<p>{{ i }}</p>
<p v-if='jender'>man</p>
<p v-else>woman</p>
<p class="customer" v-for="customer in customers" :key="customer.id">{{ customer.name }} , {{ customer.city }}</p>
```


````
data: () => ({
        name: 'Hello Saeed!',
        i: 1,
        jender: true,
        customers: [
            { id: 1, name: 'saeed', city: 'Breman' },
            { id: 2, name: 'behnam', city: 'chemnitz' }
    ]
````


</script>
