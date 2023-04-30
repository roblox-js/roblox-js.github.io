<template>
  <div class="home-container">
    <app-header></app-header>
    <div class="home-hero">
      <div class="home-container1">
        <div class="home-card">
          <h1 class="home-text">Roblox.js</h1>
          <h1 class="home-text1">Easy to use and lightweight</h1>
          <span class="home-text2">
            Streamline ROBLOX API interaction with roblox.js - the easy-to-use NPM
            package.
          </span>
          <div class="home-container2">
            <div class="home-container3">
              <a
                href="https://npmjs.com/package/roblox.js"
                target="_blank"
                rel="noreferrer noopener"
                class="home-link"
              >
                <primary-pink-button
                  button="install"
                  class="home-component1"
                ></primary-pink-button>
              </a>
            </div>
            <a
              href="https://roblox-js.github.io/docs"
              target="_blank"
              rel="noreferrer noopener"
              class="home-link1"
            >
              <outline-gray-button
                button="documentation"
                class="home-component2"
              ></outline-gray-button>
            </a>
          </div>
        </div>
      </div>
    </div>
    <img
      alt="image"
      src="/playground_assets/curved6-1500h.jpg"
      class="home-image"
    />
    <section class="home-testimonials">
      <img
        alt="image"
        src="/playground_assets/bottom.svg"
        class="home-bottom-wave-image"
      />
      <img
        alt="image"
        src="/playground_assets/waves-white.svg"
        class="home-image1"
      />
    </section>
  </div>
</template>

<script>
import AppHeader from '../components/header'
import PrimaryPinkButton from '../components/primary-pink-button'
import OutlineGrayButton from '../components/outline-gray-button'

export default {
  name: 'Home',
  components: {
    AppHeader,
    PrimaryPinkButton,
    OutlineGrayButton,
  },
  metaInfo: {
    title: 'Roblox.js',
    meta: [
      {
        property: 'og:title',
        content: 'Roblox.js',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  height: auto;
  display: flex;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
}
.home-hero {
  width: 100%;
  display: flex;
  max-width: 1320px;
  padding-left: var(--dl-space-space-unitandahalfunit);
  padding-right: var(--dl-space-space-unitandahalfunit);
  justify-content: center;
}
.home-container1 {
  width: 100%;
  display: flex;
  position: relative;
  max-width: 1320px;
  min-height: 85vh;
  align-items: flex-start;
  flex-direction: column;
  justify-content: center;
}
.home-card {
  flex: 0 0 auto;
  width: 60%;
  display: flex;
  padding: var(--dl-space-space-tripleunit);
  z-index: 1;
  box-shadow: 0 8px 26px -4px hsla(0,0%,8%,.15),0 8px 9px -5px hsla(0,0%,8%,.06)!important;
  margin-top: var(--dl-space-space-tripleunit);
  align-items: flex-start;
  border-radius: var(--dl-radius-radius-radius1);
  flex-direction: column;
  backdrop-filter: saturate(200%) blur(30px);
  background-color: hsla(0,0%,100%,.8);
}
.home-text {
  text-align: center;
  background-image: linear-gradient(310deg, rgb(121, 40, 202), rgb(255, 0, 128));
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
.home-text1 {
  color: var(--dl-color-secondary-700);
  text-align: center;
  margin-bottom: var(--dl-space-space-unitandahalfunit);
}
.home-text2 {
  color: var(--dl-color-secondary-600);
  margin-right: var(--dl-space-space-tripleunit);
  margin-bottom: var(--dl-space-space-unit);
  padding-right: var(--dl-space-space-tripleunit);
}
.home-container2 {
  display: flex;
  margin-top: var(--dl-space-space-unitandahalfunit);
  align-items: flex-start;
  margin-bottom: var(--dl-space-space-unit);
  flex-direction: row;
}
.home-container3 {
  display: flex;
  align-items: flex-start;
  margin-right: var(--dl-space-space-unit);
  flex-direction: row;
}
.home-link {
  display: contents;
}
.home-component1 {
  text-decoration: none;
}
.home-link1 {
  display: contents;
}
.home-component2 {
  text-decoration: none;
}
.home-image {
  top: 0px;
  left: auto;
  right: 0px;
  width: 50%;
  bottom: 0px;
  height: 80vh;
  position: absolute;
  object-fit: cover;
  object-position: right;
  border-bottom-left-radius: 10rem;
}
.home-testimonials {
  flex: 0 0 auto;
  width: 100%;
  display: flex;
  position: relative;
  align-items: center;
  flex-direction: column;
  background-image: linear-gradient(310deg,#7928ca,#ff0080);
}
.home-bottom-wave-image {
  top: auto;
  left: auto;
  right: 0px;
  width: 100%;
  bottom: -5px;
  position: absolute;
  object-fit: cover;
}
.home-image1 {
  top: auto;
  left: 0px;
  right: 0px;
  width: 100%;
  bottom: auto;
  height: 100%;
  position: absolute;
  object-fit: cover;
}
@media(max-width: 991px) {
  .home-hero {
    padding-left: var(--dl-space-space-tripleunit);
    padding-right: var(--dl-space-space-tripleunit);
  }
  .home-container1 {
    max-width: 960px;
  }
  .home-card {
    width: 100%;
  }
}
@media(max-width: 767px) {
  .home-card {
    align-items: center;
  }
  .home-text2 {
    text-align: center;
    margin-right: 0px;
    padding-right: 0px;
  }
  .home-image {
    display: none;
  }
}
@media(max-width: 479px) {
  .home-card {
    padding: var(--dl-space-space-unit);
  }
  .home-container2 {
    align-items: center;
    flex-direction: column;
  }
  .home-container3 {
    margin-right: 0px;
    margin-bottom: var(--dl-space-space-unit);
  }
}
</style>
