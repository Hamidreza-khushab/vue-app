<template>
    <div>
        <p>Practice</p>
        <button @click="submit">submit</button>
        <p>{{ this.i }}</p>
        <input type="text" v-model="task" />
        <button @click="submitOne">submit</button>
        <p v-for="e in Tasks" :key="e">{{ e }}</p>
    </div>
</template>

<script>
export default {
    name: 'Practice',
    data: () => ({
        i: 1,
        state: true,
        task: '',
        Tasks : []
    }),
    methods: {
        submit() {
            this.i = this.i + 1
        },
        submitOne(){
           this.Tasks.push(this.task)
           this.task = ''
        }
    }
}
</script>

<style  scoped>

</style>