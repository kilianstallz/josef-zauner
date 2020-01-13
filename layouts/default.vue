<template>
  <div>
    <section class="main-bg flex flex-col">
      <img
        src="~/assets/bg-white.svg"
        alt="BG"
        class="absolute z-0 h-screen bg-image"
      />
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
      <div class="intro flex flex-col z-50">
        <span class="intro-head"
          >Consulting <br />
          Gutachten <br />
          Projektbegleitung</span
        >
        <span class="intro-sub">Alles aus einer Hand. Josef Zauner, MBA</span>
        <div class="flex flex-row cta">
          <button class="py-3 px-5 button">
            Mehr erfahren
          </button>
          <span class="my-auto pl-12">Kontakt</span>
        </div>
      </div>
      <img
        src="~/assets/certificate.svg"
        alt="Certificate"
        class="absolute cert-image"
      />
    </section>
    <section class="flex flex-col pt-24">
      <h2 style="font-size: 42px;" class="text-center">
        Gemeinsam Maßnahmen ergreifen
      </h2>
      <h2 style="font-size: 40px;" class="text-center">
        Chancen am Markt warnehmen
      </h2>
      <!-- Leistungen Rows -->
      <div class="leistungen">
        <!-- 1 -->
        <div class="leistungen_row flex row">
          <div class="leistungen_text">
            <h3>Consulting</h3>
            <p>
              Ich unterstütze Sie beim Fortschritt in der Unternehmens-,
              Produktions- und Einkaufsorganisation.
            </p>
            <nuxt-link to="/consulting">
              Mehr erfahren ->
            </nuxt-link>
          </div>
          <img
            src="~/assets/undraw_quiz_nlyh.svg"
            alt="Quiz"
            class="leistungen_img"
          />
        </div>
        <!-- 2 -->
        <div class="leistungen_row flex row">
          <div class="leistungen_text">
            <h3>Gutachten</h3>
            <p>
              Ich bin allgemein beeideter und gerichtlich zertifizierter
              Sachverständiger. Ich erstelle Privat- und Gerichtsgutachten.
            </p>
            <nuxt-link to="/gutachten">
              Mehr erfahren ->
            </nuxt-link>
          </div>
          <img
            src="~/assets/undraw_confirmation_2uy0.svg"
            alt="Gutachten"
            class="leistungen_img"
          />
        </div>
        <!-- 3 -->
        <div class="leistungen_row flex row">
          <div class="leistungen_text">
            <h3>Projektbegleitung</h3>
            <p>
              Ich unterstütze den Metallbauer bei der Entwicklung rationeller
              Detaillösungen.
            </p>
            <nuxt-link to="/begleitung">
              Mehr erfahren ->
            </nuxt-link>
          </div>
          <img src="~/assets/folder.svg" alt="Folder" class="leistungen_img" />
        </div>
      </div>
    </section>
    <!-- <nuxt /> -->
  </div>
</template>

<script>
export default {
  name: 'Home'
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}

.bg-image {
  height: 100vh;
}

.cert-image {
  right: 44px;
  top: 150px;
  width: 50%;
}

.main-bg {
  background: #9bfaf5;
  height: 100vh;
  width: 100%;
}

.intro {
  margin-left: 150px;
  margin-top: 120px;
}
.intro-head {
  font-size: 48px;
  margin-bottom: 45px;
  font-weight: 500;
}
.intro-sub {
  font-size: 18px;
  margin-bottom: 45px;
  font-weight: 500;
}

.button {
  background: #ff4f4f;
  color: #fff;
  font-weight: 500;
}

.cta > span {
  font-weight: 500;
  color: #333;
}

/**
* Leistungen
 */

.leistungen {
  max-width: 890px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
}

.leistungen_row {
  margin-top: 120px;
  display: flex;
  justify-content: space-between;
}
.leistungen_row:nth-child(2n) {
  flex-direction: row-reverse;
}

.leistungen_text h3 {
  font-size: 40px;
  font-weight: 500;
  margin-bottom: 16px;
}
.leistungen_text p {
  font-size: 18px;
  margin-bottom: 26px;
  max-width: 360px;
}
.leistungen_text a {
  color: #2979ff;
}

.leistungen_img {
  width: 40%;
}
</style>
