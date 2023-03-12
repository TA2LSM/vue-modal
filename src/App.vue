<!-- This is main route component (App.vue) -->
<!-- Template is a mandatory part -->
<template>
  <h1>{{title}}</h1><br>
  <input type="text" ref="name">
  <button @click="handleClick">Click me!</button>
  <Modal />
</template>


<!--  These below are optional -->
<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
   
  components: {
    Modal
  },

  data() {
    return {
      title: "~ First Vue Project ~"
    }
  },

  methods: {
    handleClick() {
      // using "refs"
      // console.log(this.$refs.named);
      // console.log(this.$refs.name.value);
      // this.$refs.name.classList.add('active');
      // this.$refs.name.focus();
    }
  },
}
</script>

<!-- These styles below will be injected in head section in html file -->
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

h1 {
  border-bottom: 1px solid #ddd;
  display: inline-block;
  padding-bottom: 10px;
}
</style>
