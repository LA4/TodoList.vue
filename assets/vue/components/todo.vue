<template>
    <div class="todo-container">

        ceci est une tâche {{ todoTitle }}
    </div>
</template>
<script>
export default {
    props: {
        showTodo: ""
    },
    data() {
        return {
            todoTitle: this.showTodo
        }
    }
}
</script>
<style scoped>
.todo-container {
    display: flex;
    width: 200px;
    height: 150px;
    background-color: #81aa84;
}
</style>