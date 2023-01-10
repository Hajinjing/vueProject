<template>
  <header>
    <Logo />
    <b-nav tabs>
      <div
        v-for="nav in navigators"
        :key="nav.name"
        class="nav-item">
        <RouterLink
          :to="nav.href"
          active-class="active"
          class="nav-link">
          {{ nav.name }}
        </RouterLink>
      </div>
    </b-nav>
  </header>
</template>

<script>
import Logo from '@/components/Logo.vue'

export default {
  name: 'Header',
  components: {Logo},
  data () {
    return {
      navigators: [
        {
          name: 'Search',
          href: '/'
        },
        {
          name: 'Movie',
          href: '/movie'
        },
        {
          name: 'About',
          href: '/about'
        }
      ]
    }
  }
}
</script>

<style scoped>
  header {
    height: 70px;
    padding: 0 40px;
    display: flex;
    align-items: center;

  }
  .logo {
    margin-right: 40px;
  }
</style>
