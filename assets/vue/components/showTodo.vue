<template>
    <div class="todos-container">
        <todo :showTodo="showTodo"></todo>
        {{ showTodo }}
    </div>
</template>
<script>
import todo from './todo.vue'
export default {
    components: {
        todo,
    },
    props: {
        showTodo: ""
    },
}
</script>
<style scoped>
.todos-container {
    display: flex;
    width: 80%;
    height: 100vh;
    background-color: #A2A2A2;
}
</style>