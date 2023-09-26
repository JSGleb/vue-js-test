<template>
  <div id="app">
    <!-- <HelloWorld msg="Hello, world."/>
    <PictureComp />
    <TestComp num="10"/> -->
    <ClasesStyles />
    <InlineStyles />
    <CompStyles />
  </div>
</template>

<script>
// import HelloWorld from './components/HelloWorld.vue'
// import PictureComp from './components/Picture.vue'
// import TestComp from './components/Test.vue'
import ClasesStyles from './components/ClassesStyles.vue'
import InlineStyles from './components/InlineStyles.vue'
import CompStyles from './components/CompStyles.vue'

export default {
  name: 'App',
  components: {
    // HelloWorld,
    // PictureComp,
    // TestComp,
    ClasesStyles,
    InlineStyles,
    CompStyles
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  /* color: red;
  background-color: purple; */
  margin-top: 60px;
  padding: 100px;
  font-size: 2em;
}
</style>
