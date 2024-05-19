<template>
    <div class="grandchild">
      <h2>Grandchild Component</h2>
      <textarea name="" id="" cols="20" rows="10">{{ message }}</textarea>
    </div>
  </template>
  
  <script>
  export default {
    name: 'GrandchildComponent',
    data() {
      return {
        message: 'This is the Grandchild Component'
      }
    },
    methods: {
      sendMessageToChild() {
        this.$emit('grandchildEvent', 'This is the Grandchild Component');
      },
    },
  };
  </script>
  
  <style scoped>
  
  .grandchild {
    padding: 20px;
    border: 25px solid #ee00ff;
    border-radius: 100px;
    margin-top: 15px;
    background-color: #d900ff;
    transition: all 0.3s ease;
  }
  .grandchild:hover {
    background-color: #ee00ff;
  }
  
  button {
    padding: 10px 20px;
    background-color: #b300ff;
    color: #050202;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.2s ease;
  }
  
  button:hover {
    background-color: #cc00ff;
  }
  
  textarea {
    width: 95%;
    padding: 10px;
    font-family: 'Times New Roman', Times, serif;
    font-size: 18px;
    border: 1px solid #e100ff;
    border-radius: 15px;
    resize: vertical;
    margin-bottom: 10px;
    text-align: center;
    background-color: #ae00ff;
    color: #ffffff;
    height: 100px;
  }
  
  h2 {
    font-size: 20px;
  }
  
  </style>