<template>
  <div class="home">
    <HeaderComp title="AP Myth Journal"/>
    <APMythBody/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeaderComp from '@/components/HeaderComp.vue'
import APMythBody from '@/components/APMythF/APMythBody.vue'

export default {
  name: 'APMythView',
  components: {
    HeaderComp,
    APMythBody
  }
}
</script>

<style>
.home {
  display: flex;
  flex-direction: column;
}
</style>
