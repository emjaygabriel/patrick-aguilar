<template>
    <section id="gallery-item">
        <div id="galleries">
            <img src="img/3274387.2749a43b.webp" />
        </div>
    </section>
  </template>
  
  <script>
  export default {
    name: 'GalleryItem',
    props: {
    //   alt: String
    }
  }
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
  <style scoped>
    #gallery-item {
        height: 800px;
        width: 100%;
    }
    #galleries img {
        width: 100%;
        object-fit: cover; /* Make the image cover the container */
        position: absolute;
        top: 0;
        left: 0;
        z-index: -1; /* Send the image to the background */
    }
  </style>
  