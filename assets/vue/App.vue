<template>
    <navbar></navbar>
    <addTodo @todo="takeTodo"></addTodo>
    <main class="main-container">
        <asideList></asideList>
        <showTodo :showTodo="todo"></showTodo>
    </main>
</template>
<script>
import navbar from './components/navbar.vue'
import asideList from './components/asideList.vue'
import showTodo from './components/showTodo.vue'
import addTodo from './components/addTodo.vue'
export default {
    components: {
        navbar,
        asideList,
        showTodo,
        addTodo
    },
    data() {
        return {
            todo: ""
        }
    },
    methods: {
        takeTodo(todo) {
            this.todo = todo
        }
    }

}
</script>
<style>
* {
    margin: 0;
    padding: 0;
}

body {
    font-family: Verdana, Geneva, Tahoma, sans-serif;
}

li {
    list-style: none;
}

.main-container {
    display: flex;
}
</style>
