<template>
    <main id="profile-page">
        <h1>Home</h1>
        <p>This is the Home page</p>
        <img src="../assets/logo.png" alt="">
	</main>
    <li v-for="item in items">
  {{ item.message }}
</li>
</template>

<script>
export default {
    name: "Home",
    data() {
        return {
            items: [{ message: 'Foo' }, { message: 'Bar' }]
        }
    }
}
</script>

<style lang="scss" scoped>
    main {
        margin-top: 120px;
        text-align: center;
    }
</style>