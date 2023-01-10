<template>
  <div class="container">
    <input
      v-model="title"
      type="text"
      placeholder="Search for Movies, Sereies & more" />
  </div>
</template>

<script>
export default {
  data () {
    return {
      title: ''
    }
  },
  name: 'Search'
}
</script>

<style scoped>

</style>
