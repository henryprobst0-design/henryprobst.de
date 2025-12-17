<script setup>
import { ref, onBeforeMount } from 'vue'
import { useDark, useToggle } from '@vueuse/core'

const isNavbarOpen = ref(true)

onBeforeMount(() => {
  if (document.body.clientWidth < 768) {
    isNavbarOpen.value = false
  }
})

const isDark = useDark({
  selector: 'body',
  attribute: 'class',
  valueDark: 'dark',
  valueLight: 'light',
})

const toggleDark = useToggle(isDark)
</script>

<template>
  <nav>
    <!-- BRAND -->
    <div class="navbar__brand italic text-center flex justify-center py-3 px-8">
      <div class="w-1/3"></div>

      <h3 class="w-1/3 text-xl my-0 flex items-center justify-center">
        <router-link
          to="/"
          class="decoration-none dark:text-white!"
        >
          Henry Probst
        </router-link>
      </h3>

      <div class="w-1/3 flex justify-end gap-3 items-center">
        <!-- DARK MODE TOGGLE (MOBILE) -->
        <a
          href="#"
          class="navbar__link p-2! md:hidden block"
          @click.prevent="toggleDark()"
        >
          <div
            class="i-mdi-theme-light-dark text-xl
                   text-gray-900 dark:text-gray-100
                   hover:text-gray-600 dark:hover:text-gray-300"
          ></div>
        </a>

        <!-- MENU TOGGLE (MOBILE) -->
        <button
          class="navbar__link p-2! md:hidden block"
          type="button"
          aria-label="Toggle Menu"
          @click="isNavbarOpen = !isNavbarOpen"
        >
          <div
            class="i-mdi-menu text-xl
                   text-gray-900 dark:text-gray-100
                   hover:text-gray-600 dark:hover:text-gray-300"
          ></div>
        </button>
      </div>
    </div>

    <!-- MENU -->
    <div class="navbar__menu">
      <ul
        v-show="isNavbarOpen"
        class="flex list-none gap-5 justify-center p-0
               flex-col md:flex-row text-right pr-8
               lg:p-0 lg:text-center"
      >
        <li class="navbar__item">
          <nuxt-link to="/" class="navbar__link">Über mich</nuxt-link>
        </li>

        <li class="navbar__item">
          <nuxt-link to="/erfolge" class="navbar__link">Erfolge</nuxt-link>
        </li>

        <li class="navbar__item">
          <nuxt-link to="/kontakt" class="navbar__link">Kontakt</nuxt-link>
        </li>

        <!-- DARK MODE TOGGLE (DESKTOP) -->
        <li class="navbar__item hidden md:block">
          <a
            href="#"
            class="navbar__link p-0!"
            @click.prevent="toggleDark()"
          >
            <div
              class="i-mdi-theme-light-dark text-xl
                     text-gray-900 dark:text-gray-100
                     hover:text-gray-600 dark:hover:text-gray-300"
            ></div>
          </a>
        </li>
      </ul>
    </div>
  </nav>
</template>

<style lang="postcss">
.navbar__link {
  padding: 0.5rem;
  text-decoration: none;
}

.navbar__link.router-link-active {
  @apply dark:text-gray-50;
  border-bottom: 1px solid;
}
</style>
