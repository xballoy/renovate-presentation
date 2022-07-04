<template>
  <footer
      v-if="$slidev.nav.currentLayout !== 'intro-image'"
      class="absolute bottom-0 left-auto right-0 p-2"
  >
    {{ $slidev.nav.currentPage }} / {{ $slidev.nav.total }}
  </footer>
</template>
