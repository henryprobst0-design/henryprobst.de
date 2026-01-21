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

<div class="flex justify-center my-8">
  <img
    src="/assets/IMG_2593.jpeg"
    alt="Henry Probst"
    class="max-w-[200px] w-full h-auto rounded-lg"
  >
</div>
      
<div class="cards max-w-[300px] mx-auto">
  <div class="contact | flex items-center justify-center mb-2">
    <div class="i-mdi-gmail w-6 h-6 bg-red-500 mr-2"></div>
    <a href="mailto:kontakt@henryprobst.de">kontakt@henryprobst.de</a>
  </div>
  <div class="contact | flex items-center justify-center">
    <div class="i-mdi-linkedin w-6 h-6 bg-blue-500 mr-2"></div>
    <a href="https://linkedin.com/in/henry-probst-1b8420389" target="_blank">Henry Probst</a>
  </div>
</div>
    </div>
  </div>
</section>
</template>
