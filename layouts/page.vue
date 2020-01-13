<template>
  <div style="min-height: 100vh;">
    <header class="flex row p-10 z-50">
      <div class="logo flex pr-24">
        <img src="~/assets/Logo.svg" alt="Logo" class="pr-4" />
        <div style="font-size: 14px;" class="flex font-semibold flex-col">
          <span>Josef Zauner</span>
          <span>Consulting</span>
        </div>
      </div>
      <nav class="font-semibold">
        <nuxt-link to="/" class="cursor-pointer pr-12">Leistungen</nuxt-link>
        <nuxt-link to="/" class="cursor-pointer pr-12">Über Mich</nuxt-link>
        <nuxt-link to="/" class="cursor-pointer pr-12">Kontakt</nuxt-link>
        <nuxt-link to="/" class="cursor-pointer">Blog</nuxt-link>
      </nav>
    </header>
    <main class="container">
      <nuxt />
    </main>
  </div>
</template>

<style scoped>
.container {
  max-width: 890px;
  margin: 0 auto;
}
</style>
