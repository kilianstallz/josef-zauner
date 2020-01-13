<script>
export default {
  name: 'MatchingIntro',
  layout: 'matching'
}
</script>

<template>
  <div class="flex flex-row">
    <div class="container text-center">
      <h3 class="mt-32">Willkommen!</h3>
      <p style="max-width: 460px;" class="text-lg mx-auto my-10">
        Nach der Reihe werden dir nun verschiedene Worte angezeigt. Wähle das
        Wort aus, dem du am meisten Bedeutung schenkst.
      </p>
      <button class="py-3 px-5 button">
        Los geht's!
      </button>
    </div>
  </div>
</template>

<style scoped>
h3 {
  font-size: 40px;
  font-weight: 500;
}
.container {
  width: 890px;
  margin: 0 auto;
  height: 100%;
}
</style>
