<template>
  <div
    class="flex flex-col h-screen justify-between bg-cover bg-center h-screen w-screen pl-6 pr-6 pt-6"
  >
    <header class="h-40 pl-6 text-left">
      <div>
        <span class="text-4xl font-bold">Jon Hose</span>
        <span class="text-xl pl-6">/\ software engineer</span>
      </div>
    </header>
    <main class="mb-auto h-40">
      <router-view />
    </main>
    <Footer />
  </div>
</template>

<script>
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Footer
  }
};
</script>

<style scoped>
.bg-cover {
  background-image: url("./assets/desk-purple-cropped.png");
  background-size: cover;
  background-position: top;
  background-repeat: no-repeat;
  font-family: "Lucida Console", Monaco, monospace;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
  background-color: black;
}
</style>
