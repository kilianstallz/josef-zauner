<template>
  <div>
    <section class="main-bg flex flex-col">
      <header class="flex row p-10">
        <div class="logo flex pr-24">
          <img src="~/assets/Logo.svg" alt="Logo" class="pr-4" />
          <div style="font-size: 14px;" class="flex font-semibold flex-col">
            <span>Josef Zauner</span>
            <span>Consulting</span>
          </div>
        </div>
        <nav class="font-semibold">
          <span class="pr-12">Leistungen</span>
          <span class="pr-12">Über Mich</span>
          <span class="pr-12">Kontakt</span>
          <span>Blog</span>
        </nav>
      </header>
      <div class="intro flex flex-col">
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
    <nuxt />
  </div>
</template>

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
  top: 120px;
}

.main-bg {
  background: #9bfaf5;
  background-image: url('~assets/bg-white.svg');
  background-repeat: no-repeat;
  background-size: 100vh;
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
</style>
