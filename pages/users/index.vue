<template>
  <div>
    <h1>user page</h1>
    <label>
      <input type="text" v-model="userId">
    </label>
    <button @click="onLoadUser">Load User</button>
  </div>

</template>

<script>
    export default {
        name: "users.vue",
        data() {
          return {
            userId: ''
          }
        },
        methods: {
          onLoadUser() {
            this.$router.push('/users/' + this.userId)
          }
        }
    }
</script>

<style scoped>

</style>
