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
  <div class="profile-wrapper">
    <img src="/assets/henryprobst.jpg" alt="Henry Probst" />

    <div class="contacts">
      <div class="contact">
        <div class="i-mdi-gmail icon gmail"></div>
        <a href="mailto:kontakt@henryprobst.de">
          kontakt@henryprobst.de
        </a>
      </div>

      <div class="contact">
        <div class="i-mdi-linkedin icon linkedin"></div>
        <a
          href="https://linkedin.com/in/henry-probst-1b8420389"
          target="_blank"
        >
          Henry Probst
        </a>
      </div>
    </div>
  </div>
</template>

      <style scoped>
.profile-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
}

.contacts {
  width: 300px;
  text-align: center;
  margin-top: 1rem;
}

.contact {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  margin-bottom: 0.5rem;
}

.icon {
  width: 24px;
  height: 24px;
}

.gmail {
  background-color: #ef4444;
}

.linkedin {
  background-color: #3b82f6;
}
</style>

