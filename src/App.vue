<template>
  <h1>{{ title }}</h1>
  <p> Welcome...</p>
  <div v-if="showModal">
    <Modal theme="sale" @close="toggleModal">
      <h1>Ninja Giveaways</h1>
      <p>Grab your ninja swag for</p>
    
    </Modal>
  </div>
 <button @click="toggleModal"> open modal </button>
</template>

<script>
import Modal from './components/Modal.vue'

export default {
  name: 'App',
  components: {Modal},
  
  data() {
    return {
      title: 'My first Vue.js!',
      header: 'Sign up for giveaways',
      text: 'Must be nice',
      showModal: false
    }
  },
  methods: {
    toggleModal() {
      this.showModal = !this.showModal;
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