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

      <img src="https://media.licdn.com/dms/image/v2/D4E03AQHPewHFiaVW0A/profile-displayphoto-crop_800_800/B4EZnJ05QgIoAI-/0/1760027710905?e=1767225600&v=beta&t=kYb7JCK7deiGlnNTsLDChy25egm2yV2hyVHWfNvZFxk" alt="Henry Probst">

      <div class="cards max-w-[300px] mx-auto">
        <div class="contact | flex items-center gap-3 mb-5">
          <div class="i-mdi-gmail w-6 h-6 bg-red-500"></div>
          <a href="mailto:kontakt@henryprobst.de">kontakt@henryprobst.de</a>
        </div>
        <div class="contact | flex items-center gap-3 mb-5">
          <div class="i-mdi-linkedin w-6 h-6 bg-blue-500"></div>
          <a href="https://linkedin.com/in/henry-probst-1b8420389" target="_blank">Henry Probst</a>
        </div>
      </div>
    </div>
  </div>
</section>
</template>
