<script setup>
import { RouterView } from 'vue-router'

</script>

<template>
  <header>

    <h1 id="mainTitle">SEPHORA</h1> 
    <img alt="Vue logo" class="logo" src="https://play-lh.googleusercontent.com/L7x1kdNfnrhGSjUYDJJ57KBbsrFirIqnkyKJ6qaIN7lSggjVsS4Knz3n07vtQYbWQiU" width="125" height="125" />

    <div class="wrapper">
      <RouterView />

    </div>
  </header>

</template>

<style scoped>
header {
  display: flex;
  flex-direction: column;
  align-items: center;
  line-height: 1.5;
  max-height: 100vh;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
  border-radius: 1rem;
}

#mainTitle{
  font-family: "Dosis", sans-serif;
}

</style>
