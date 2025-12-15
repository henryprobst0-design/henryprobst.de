<script setup>
useHead({
  titleTemplate: (titleChunk) => {
    return titleChunk ? `${titleChunk} - Henry Probst` : 'Henry Probst';
  },
  htmlAttrs: {
    lang: 'de'
  },
  meta: [
    { hid: 'description', name: 'description', content: 'Webseite von Henry Probst' }
  ]
})
</script>
<template>
  <div id="app" class="min-h-screen">
    <NuxtLayout>
      <NuxtPage/>
    </NuxtLayout>
  </div>
</template>
