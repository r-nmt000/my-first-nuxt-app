<template>
  <div>
    <Header></Header>
    <header>User Section</header>
    <nuxt />
  </div>
</template>

<script>
    import Header from "~/components/Header.vue"
    export default {
        name: "users.vue",
      components: {Header}
    }
</script>

<style scoped>

</style>
