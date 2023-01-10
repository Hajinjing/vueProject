<template>
  <RouterLink
    to="/"
    class="logo">
    <span class="llgo">OMDBAPI</span>.COM
  </RouterLink>
</template>

<script>
export default {
  name: 'Logo'
}
</script>

<style scoped>

.logo {
  font-family: 'Oswald', sans-serif;
  font-size: 20px;
  color: black;
}
.llgo {
  font-family: 'Oswald', sans-serif;
  color: chocolate;
  font-size: 20px;
}
</style>
