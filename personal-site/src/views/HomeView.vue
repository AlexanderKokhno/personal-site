<template>
  <div class="home">
    <HeaderComp title="Home"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/HeaderComp.vue'

export default {
  name: 'HomeView',
  components: {
    HeaderComp
  }
}
</script>
