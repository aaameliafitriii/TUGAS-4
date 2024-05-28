<template>
    <div>
      <h3>Child Two</h3>
      <button @click="sendData">Send Data to Parent</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'childtwo',
    methods: {
      sendData() {
        this.$emit('data-from-child', 'Data from child two');
      }
    }
  }
  </script>