<template>
    <div class="addtodo-container">
        <label for="addtodo">Ajouter une tâche</label>
        <div class="addtodo-input-container">
            <input v-model="textTodo" class="addtodo-input" id="addtodo" type="text" placeholder="notez votre tâche">
            <button @click="addTodo" class="addtodo-button">+</button>
        </div>


    </div>
</template>
<script>
export default {

    data() {
        return {
            textTodo: "",
        }
    },
    methods: {

        addTodo(e) {
            e.preventDefault()
            this.$emit('todo', this.textTodo)
            this.textTodo = ''
        }

    }

}
</script>
<style>
.addtodo-container {
    display: flex;
    width: 400px;
    justify-content: center;
    flex-direction: column;
    gap: 10px;
    margin: 50px auto;

}

.addtodo-input-container {
    display: flex;
    width: 100%;
}

.addtodo-input {
    display: block;
    width: 80%;
}

.addtodo-button {
    display: block;
    width: 25px;
    height: 25px;
}
</style>