<template>
  <div class="home">
    <HeaderComp msg="AP Mythology Journal"/>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component'
import HeaderComp from '@/components/HeaderComp.vue' // @ is an alias to /src

@Options({
  components: {
    HeaderComp
  },
  data () {
    return {
      APMythImg: 'Achilles.png'
    }
  }
})
export default class APMyth extends Vue {}
</script>
