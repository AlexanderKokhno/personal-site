
<template>
  <div class="APMythPost">
    <p>TESTING TESTING</p>
    <div class="titleRow">
      <h1 >{{ postEntrie.date }}</h1>
    </div>
    <div class='bodyRow'>
      <p>{{postEntrie.bodyText}}</p>
    </div>

  </div>
</template>
/* eslint-disable */
<script>
export default {
  name: 'APMythPosts',
  props: ['postEntrie']
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import '@/assets/style.css';
.APMythPost {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: auto;
  border-style: solid;
  border-radius: 25px;
}

.titleRow {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 1vh;
  color: black;
}
.bodyRow {
  flex-direction: row;
  width: 100%;
  justify-content: center;
  padding: 1vh;
}

</style>
