<script setup>
definePageMeta({
  layout: "main",
});
useHead({
  title: 'Erfolge',
})

const achievements = [
  {
    text: '2025-vorraussichtlich 2028',
    class: 'i-mdi:trophy text-yellow-500 w-6 h-6',
    description: `Ausbildung als IT-Systemelektroniker bei Technogroup/Evernex`
  },
  {
    text: '2025-vorraussichtlich 2028',
    class: 'i-mdi:trophy text-yellow-500 w-6 h-6',
    description: `Berufsschulunterricht Friedrich-Ebert-Schule in Wiesbaden`
  },
  {
    text: '2024',
    class: 'i-mdi:trophy text-yellow-500 w-6 h-6',
    description: `Realschulabschluss mit Note 2,5 in Hessen`
  },
]
</script>
<template>
<section class="content">
  <div class="container mx-auto">
    <div class="section__header | text-center">
      <h1 class='section__title'>Erfolge</h1>
    </div>
    <ul class="pl-0 list-none">
      <li v-for="achievement in achievements" class="achievement-item mb-5">
        <div class="achievement-name list-none flex gap-3 items-center ">
          <div :class="achievement.class"></div>
          <span class="font-bold text-lg">
            {{achievement.text}}
          </span>
        </div>
        <div class="achievement-description pl-10 py-5 leading-loose dark:opacity-80" v-html="achievement.description.replaceAll(new RegExp('\n', 'g'), '<br/>')">
        </div>
      </li>
    </ul>
  </div>
</section>
</template>
