<template>
   <h1>a single user, with ID: {{ $route.params.id }}</h1>
</template>

<script>
    export default {
        name: "_id",
        validate(data) {
          return /^[0-9]+$/.test(data.params.id)
        },
        layout: 'users'
    }
</script>

<style scoped>

</style>
