<template>
    <section id="header">
        <a href="#"><img src="https://placehold.co/100x80?text=Logo" /></a>
    </section>
  </template>
  
  <script>
  export default {
    name: 'HeaderItem',
    props: {
    //   alt: String
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    #header {
        padding-top: 0.5rem;
        padding-bottom: 0.5rem;
        background-color: #1D5D9B;
    }
  </style>
  