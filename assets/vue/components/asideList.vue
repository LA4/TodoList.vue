<template>
    <aside class="aside-list-container">
        <span>Listes des tâches en cours</span>
        <div class="aside-list-items-container">
            <ul>
                <li>premiere tâche</li>
                <li>seconde tâche</li>
            </ul>
        </div>
    </aside>
</template>
<script>
export default {

}
</script>
<style scoped>
.aside-list-container {
    display: flex;
    flex-direction: column;
    gap: 50px;
    padding: 10px;
    width: 200px;
    height: 100vh;
    background-color: #CECECE;
}

.aside-list-items-container {
    display: flex;
}
</style>