<template>
    <nav>
        <img src="" alt="ironhack logo" class="iron-logo">
        <img src="" alt="ironhack menu" class="menu">
    </nav>
</template>

<script>
export default {
    name: "NavBar"
}
</script>

<style scoped>
nav {
    display: flex;
    justify-content: space-between

}

.iron-logo {
    width: 35px;
    height: 38px;
    margin-left: 30px;
    margin-top: 20px;

}

.menu {
    width: 22px;
    height: 20px;
    margin-right: 30px;
    margin-top: 29px;

}
</style>