<template>
  <HeaderItem></HeaderItem>
  <GalleryItem></GalleryItem>
  <SectionItem :alt="false">
    <h2>About</h2>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam urna sapien, placerat vel tincidunt blandit, volutpat eu tortor. Etiam varius, mauris non malesuada interdum, ante sem efficitur libero, ac malesuada lacus massa ut elit. Fusce fermentum purus quis neque mollis lobortis. Integer at est ac justo egestas lobortis ac vel ante. Morbi posuere aliquet purus, non mollis est dictum eget. Sed quis ipsum sed tellus fringilla posuere. Vivamus dui augue, iaculis ac aliquet dapibus, lobortis fermentum magna. Donec malesuada bibendum sem at congue. Nulla aliquam et leo non pellentesque. In at tortor ut tellus posuere finibus quis sed neque. Etiam in euismod eros. Nullam et tempus tortor. Praesent commodo ante lorem, ac suscipit ipsum mollis eget. Aenean et metus in elit luctus porttitor sagittis ut lorem. Nulla felis metus, rhoncus eget felis eget, finibus placerat ante. Curabitur accumsan, metus ac gravida ultricies, ipsum ex tincidunt ex, ac viverra nisi velit faucibus sapien.</p>

    <p>Etiam efficitur tempor molestie. Curabitur sit amet enim ipsum. Nullam ut ligula eget lacus aliquet euismod. In interdum, felis at commodo euismod, nunc elit dignissim dui, ac aliquet tortor metus nec massa. Aenean in interdum nisi. Suspendisse in eros ac velit pretium porta vel vel turpis. Proin pellentesque dolor nisl, et pharetra nibh hendrerit in. Nulla a massa ultricies, consequat enim ut, tempus erat. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce at ullamcorper eros, ut accumsan ante. Etiam id arcu vitae erat vulputate fermentum nec quis urna. Aenean luctus egestas accumsan. Donec a laoreet nulla, at aliquam nibh. Ut auctor, nibh ac mattis sollicitudin, diam leo ornare velit, quis ultrices purus justo sed nulla.</p>
  </SectionItem>
  <SectionItem :alt="true">
    <h2>Equipments</h2>
    <div class="container">
      <div class="row equipment-item">
        <div class="col-lg-4">
          <img src="https://placehold.co/800x600?text=Equipment Image" style="width: 100%;" />
        </div>
        <div class="col-lg-8">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam urna sapien, placerat vel tincidunt blandit, volutpat eu tortor. Etiam varius, mauris non malesuada interdum, ante sem efficitur libero, ac malesuada lacus massa ut elit. Fusce fermentum purus quis neque mollis lobortis. Integer at est ac justo egestas lobortis ac vel ante. Morbi posuere aliquet purus, non mollis est dictum eget. Sed quis ipsum sed tellus fringilla posuere. Vivamus dui augue, iaculis ac aliquet dapibus, lobortis fermentum magna. Donec malesuada bibendum sem at congue. Nulla aliquam et leo non pellentesque. In at tortor ut tellus posuere finibus quis sed neque. Etiam in euismod eros. Nullam et tempus tortor. Praesent commodo ante lorem.</p>
        </div>
      </div>
      <div class="row equipment-item">
        <div class="col-lg-8 order-lg-1 order-sm-2 order-xs-2">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam urna sapien, placerat vel tincidunt blandit, volutpat eu tortor. Etiam varius, mauris non malesuada interdum, ante sem efficitur libero, ac malesuada lacus massa ut elit. Fusce fermentum purus quis neque mollis lobortis. Integer at est ac justo egestas lobortis ac vel ante. Morbi posuere aliquet purus, non mollis est dictum eget. Sed quis ipsum sed tellus fringilla posuere. Vivamus dui augue, iaculis ac aliquet dapibus, lobortis fermentum magna. Donec malesuada bibendum sem at congue. Nulla aliquam et leo non pellentesque. In at tortor ut tellus posuere finibus quis sed neque. Etiam in euismod eros. Nullam et tempus tortor. Praesent commodo ante lorem.</p>
        </div>
        <div class="col-lg-4 order-lg-2 order-sm-1 order-xs-1">
          <img src="https://placehold.co/800x600?text=Equipment Image" style="width: 100%;" />
        </div>
      </div>
      <div class="row equipment-item">
        <div class="col-lg-4">
          <img src="https://placehold.co/800x600?text=Equipment Image" style="width: 100%;" />
        </div>
        <div class="col-lg-8">
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam urna sapien, placerat vel tincidunt blandit, volutpat eu tortor. Etiam varius, mauris non malesuada interdum, ante sem efficitur libero, ac malesuada lacus massa ut elit. Fusce fermentum purus quis neque mollis lobortis. Integer at est ac justo egestas lobortis ac vel ante. Morbi posuere aliquet purus, non mollis est dictum eget. Sed quis ipsum sed tellus fringilla posuere. Vivamus dui augue, iaculis ac aliquet dapibus, lobortis fermentum magna. Donec malesuada bibendum sem at congue. Nulla aliquam et leo non pellentesque. In at tortor ut tellus posuere finibus quis sed neque. Etiam in euismod eros. Nullam et tempus tortor. Praesent commodo ante lorem.</p>
        </div>
      </div>
    </div>
  </SectionItem>
  <SectionItem :alt="false">
    <h2>Contact</h2>
    <form class="standard-form">
        <div class="field">
          <label for="email">Email:</label>
        <input type="email" id="email" name="email" required>
        </div>
        <div class="field">
        <label for="subject">Subject:</label>
        <input type="text" id="subject" name="subject" required>
        </div>
        <div class="field">
        <label for="message">Message:</label>
        <textarea id="message" name="message" rows="4" cols="50" required></textarea>
      </div>
      <div class="field">
        <a id="sendEmailLink" href="#">Send Email</a>
        </div>
    </form>

  </SectionItem>
</template>

<script>
import SectionItem from './components/section-item.vue';
import HeaderItem from './components/header-item.vue';
import GalleryItem from './components/gallery-item.vue';


export default {
  name: 'App',
  components: {
    HeaderItem,
    SectionItem,
    GalleryItem
  },
  mounted() {
    document.getElementById("sendEmailLink").addEventListener("click", function () {
          var email = document.getElementById("email").value;
          var subject = encodeURIComponent(document.getElementById("subject").value);
          var message = encodeURIComponent(document.getElementById("message").value);
          var mailtoLink = "mailto:" + email + "?subject=" + subject + "&body=" + message;
          window.location.href = mailtoLink;
      });
  }
}
</script>

<style>
html, body {
  margin: 0;
  padding: 0;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

.section .section-container {
    margin: 0 auto;
    max-width: 1280px;
    min-width: 240px;
} 

.section h1, .section h2, .section h3 {
    text-align: center;
    margin-bottom: 3rem;
}

.section h2 {
  font-size: 2.5rem;
}

.section p {
    margin-bottom: 2rem;
    line-height: 1.5;
    text-align: left;
    font-size: 1.3rem;
}

.equipment-item {
  margin-bottom: 3rem;
}
.equipment-item:last-child {
  margin-bottom: 3rem;
}
form.standard-form {
    width: 80%;
    max-width: 400px;
    margin: 0 auto;
}

form.standard-form .field {
  margin-bottom: 1rem;
}

form.standard-form label {
    display: block;
    margin-bottom: 5px;
    font-weight: bold;
    text-align: left;
}

form.standard-form input[type="email"],
form.standard-form input[type="text"],
form.standard-form textarea {
    width: 100%;
    padding: 8px;
    margin-bottom: 10px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

form.standard-form input[type="submit"] {
    background-color: #007bff;
    color: #fff;
    padding: 10px 20px;
    border: none;
    border-radius: 25px; /* Rounded border radius */
    cursor: pointer;
    font-weight: bold;
    transition: background-color 0.3s ease-in-out;
}

form.standard-form input[type="submit"]:hover {
    background-color: #0056b3;
}

form.standard-form a {
    text-decoration: none;
    color: #007bff;
    font-weight: bold;
}
</style>
