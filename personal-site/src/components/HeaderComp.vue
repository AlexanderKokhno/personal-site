
<template>
  <div class="HeaderComp">
    <div class="HeaderRow1">
      <h1>{{ title }}</h1>
      <form class="HeaderDropDown">
        <select  onchange="showDropInfo()">
            <option ><router-link to="/">Home</router-link></option>
            <option ><router-link to="/APMyth">AP Myth Journal test</router-link></option>
            <option value="B">Option 2</option>
            <option value="C">Option 3</option>
            <router-link to="/APMyth">AP Myth Journal</router-link>
        </select>
      </form>
    </div>
    <router-link to="/">Home</router-link> |
    <router-link to="/APMyth">AP Myth Journal</router-link>
    <img alt="Vue logo" src="../assets/images/Achilles.png"/>
  </div>
</template>
/* eslint-disable */
<script>
export default {
  name: 'HeadComp',
  props: {
    title: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import '../assets/style.css';
</style>
