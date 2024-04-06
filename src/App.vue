i<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
const goToHome = () => {
  alert("button home");
}

const goToAbout = () => {
  alert("button about");
}
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/page.1.png" width="400" height="400" />

    <div class="wrapper">
      <HelloWorld msg="Hi! I'm mohd farhan.s" />
    </div>
  </header>
  <br><br>

<nav>
  <ul>
    <button @click="goToHome">Home</button>
    <button @click="goToAbout">About</button>
  </ul>
</nav>
<br><br>
  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
