
<template>
  <div class="headerComp">
    <div class="introRow">
      <h1 id='headerTitle'>{{ title }}</h1>
      <img alt="Vue logo" src="@/assets/images/Achilles.png"/>
      <!-- <form class="headerDropDown">
        <select  onchange="showDropInfo()">
            <option ><router-link to="/">Home</router-link></option>
            <option ><router-link to="/APMyth">AP Myth Journal test</router-link></option>
            <option value="B">Option 2</option>
            <option value="C">Option 3</option>
            <router-link to="/APMyth">AP Myth Journal</router-link>
        </select>
      </form> -->
    </div>
    <div class='posts'>
      <P>hfeufuuebfubeub</P>
      <div v-for='allEntrie in allEntries' :key='allEntrie'>
        <APMythPosts v-bind:postEntrie="allEntrie"/>
      </div>
    </div>

    <!-- <img alt="Vue logo" src="../assets/images/Achilles.png"/> -->
  </div>
</template>
/* eslint-disable */
<script>
import APMythPosts from '@/components/APMythF/APMythPosts.vue'
export default {

  name: 'APMythBody',
  components: {
    APMythPosts
  },
  props: {
    title: String
  },
  data () {
    return {
      allEntries: [
        {
          date: 'lorem1',
          bodyText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat perspiciatis amet molestias dolore optio odit officiis consequatur maiores, enim quibusdam facere dicta maxime repellendus architecto fuga voluptates. Eius, nesciunt pariatur?'
        },
        {
          date: 'lorem2',
          bodyText: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Repellat perspiciatis amet molestias dolore optio odit officiis consequatur maiores, enim quibusdam facere dicta maxime repellendus architecto fuga voluptates. Eius, nesciunt pariatur?'
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import '@/assets/style.css';
.headerComp {
  display: flex;
  flex-direction: column;
  width: 100%;
  height: auto;
}

.introRow {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 1vh;
}
.Posts {
  width: 100%;
  justify-content: center;
  padding: 1vh;
  border-style: solid none solid none;
}
.headerDropDown {

  padding: 1vh;
}
#headerTitle {
  border-radius: 25px;
  border-style: solid;
  padding:1vh;
}
</style>
