<template>
  <div class="hello">
    <nav>
      <p>{{msg}}</p>
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link>
    <img :src="img" alt='headerImg'/>
  </nav>
  </div>
</template>

<script >
import { Options, Vue } from 'vue-class-component'

@Options({
  props: {
    msg: String,
    img: String
  }
})
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
