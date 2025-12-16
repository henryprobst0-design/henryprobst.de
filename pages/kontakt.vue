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

<template>
  <div class="flex flex-col items-center gap-4 mt-8">
    <!-- Bild -->
    <img src="/assets/henryprobst.jpg" alt="Henry Probst" class="w-48 h-auto rounded-full" />

    <!-- Kontakte -->
    <div class="flex flex-col items-center gap-2 w-72">
      <!-- E-Mail -->
      <div class="flex items-center justify-center gap-2">
        <div class="i-mdi-gmail w-6 h-6 bg-red-500"></div>
        <a href="mailto:kontakt@henryprobst.de" class="text-blue-600 hover:underline">
          kontakt@henryprobst.de
        </a>
      </div>

      <!-- LinkedIn -->
      <div class="flex items-center justify-center gap-2">
        <div class="i-mdi-linkedin w-6 h-6 bg-blue-500"></div>
        <a href="https://linkedin.com/in/henry-probst-1b8420389" target="_blank" class="text-blue-600 hover:underline">
          Henry Probst
        </a>
      </div>
    </div>
  </div>
</template>

<script setup>
// Kein Script notwendig, nur Template + Tailwind
</script>

<style scoped>
/* Optional: zusätzliche Styles für Icons, falls du keine Tailwind-Icons hast */
.i-mdi-gmail {
  border-radius: 0.25rem;
}

.i-mdi-linkedin {
  border-radius: 0.25rem;
}
</style>



