<template>
  <div class="home">
    <img alt="Vue logo" src="">
    <HeaderComp msg="Home"/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'
import HeaderComp from '@/components/HeaderComp.vue' // @ is an alias to /src

@Options({
  components: {
    HeaderComp
  }
})
export default class HomeView extends Vue {}
</script>
