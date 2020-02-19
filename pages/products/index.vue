<template>
  <div>
    <h1>products page</h1>
    <label>
      <input type="text" v-model="productId">
    </label>
    <button @click="onLoadProduct">Load Product</button>
  </div>
</template>

<script>
    export default {
        name: "index.vue",
        data() {
          return {
            productId: ''
          }
        },
        methods: {
          onLoadProduct() {
            this.$router.push('/products/' + this.productId)
          }
        }
    }
</script>

<style scoped>

</style>
