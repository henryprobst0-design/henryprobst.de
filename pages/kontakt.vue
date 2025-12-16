<script setup>
definePageMeta({
  layout: "main",
});
useHead({
  title: 'Kontakt',
})
</script>
<template>
<section class="content">
  <div class="container mx-auto">
    <div class="prose">
      <h1 class="text-center">Kontakt</h1>

      <center>
<img src="/assets/henryprobst.jpg" alt="Henry Probst">
</center>

      <br>

      <div class="cards max-w-[300px] mx-auto">
        <div class="contact | flex items-center">
          <div class="i-mdi-gmail w-6 h-6 bg-red-500"></div>
          <a href="mailto:kontakt@henryprobst.de">kontakt@henryprobst.de</a>
        </div>
        <div class="contact | flex items-center">
          <div class="i-mdi-linkedin w-6 h-6 bg-blue-500"></div>
          <a href="https://linkedin.com/in/henry-probst-1b8420389" target="_blank">Henry Probst</a>
        </div>
      </div>
    </div>
  </div>
</section>
</template>
