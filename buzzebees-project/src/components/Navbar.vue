<template>
    <nav>
        <div class="logo">
            <img src="../assets/logo.png" alt="">
        </div>
        <ul class="menu">
            <li><router-link class="button" to="/">Profile</router-link></li>
            <li><router-link class="button" to="/gallery">Gallery</router-link></li>
        </ul>
    </nav>
</template>

<script>
export default {

}
</script>


<style lang="scss">


nav {
    display: flex;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    justify-content: space-between;
    align-items: center;
    height: 100px;
    width: 100%;
    position: fixed;
    top: 0%;
    background-image: url(../assets/buzzebees-bg.png);
}
.logo img {
    width: 3rem;
    height: 3rem;
    margin: 5px;
    border-radius: 3rem;
}
.menu {
    display: flex;
    list-style: none;
}
.menu li {
    margin: 0 2rem;
}
</style>
