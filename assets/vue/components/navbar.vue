<template>
    <nav class="nav-container">
        <h1 class="nav-logo">Todos</h1>
        <ul class="nav-items">
            <li> mes tâches </li>
            <li>creer une Tâche</li>
        </ul>
    </nav>
</template>
<script>
export default {

}
</script>
<style scoped>
.nav-container {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    width: 100%;
    height: 50px;
    background-color: #326087;
}

.nav-items {
    display: flex;
    gap: 10px;
}
</style>