<template>
  <h1>{{ title }}</h1>
  <p> Welcome...</p>
  <div v-if="showModal">
    <Modal theme="sale" @close="toggleModal">
      <template v-slot:links>
       <a href="#"> Sign up now</a>
       <a href="#"> More info</a>
      </template>
      <h1> Sign Up for GiveAways </h1>
      <p> Must be Nice </p>
    </Modal>
  </div>

  <div v-if="showModalTwo">
    <Modal theme="" @close="toggleModalTwo">

      <h1> Sign Up to our news letter </h1>
      <p> For Updates and promo codes </p>
    </Modal>
  </div>

 <button @click="toggleModal"> open modal </button>
 <button @click="toggleModalTwo"> open modalTwo</button>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {Modal},
  
  data() {
    return {
      title: 'My first Vue.js!',
      showModal: false,
      showModalTwo: false,
    }
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal;
    },
    toggleModalTwo() {
      this.showModalTwo = !this.showModalTwo;
    },
  }

}
</script>

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