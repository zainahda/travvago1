<template>
  <div class="home">
    <Navbar/>
    <Landing/>

  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from '@/components/Navbar.vue'
import Landing from '@/components/Landing.vue'

export default {
  name: 'Home',
  components: {
    Navbar,
    Landing,
  }
}
</script>
