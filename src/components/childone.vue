<template>
    <div class="child-one">
      <h3>Child One</h3>
      <button @click="sendData">Send Data to Parent</button>
    </div>
  </template>
  
  <script>
  export default {
    name: 'childone',
    methods: {
      sendData() {
        this.$emit('data-from-child', 'Data from child one');
      }
    }
  }
  </script>
  
  <style scoped>
  .child-one {
    padding: 10px;
    border: 1px solid #ccc;
    border-radius: 5px;
    background-color: #f9f9f9;
    text-align: center;
  }
  
  .child-one h3 {
    color: #2c3e50;
    margin-bottom: 10px;
  }
  
  .child-one button {
    padding: 8px 16px;
    background-color: #42b983;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
  }
  
  .child-one button:hover {
    background-color: #358a68;
  }
  </style>
  