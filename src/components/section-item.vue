<template>
    <section class="section" :class="{ 'alternate': alt == true }" >
      <div class="section-container">
        <slot></slot>
      </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'SectionItem',
    props: {
      alt: Boolean
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    .section {
        background-color: #fff;
        padding: 2rem 1.5rem;
    }
    .section.alternate {
        background-color: #75C2F6;
    }

    
  </style>
  