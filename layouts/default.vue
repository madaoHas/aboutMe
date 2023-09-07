<script lang="ts" setup></script>
<template>
  <div class="mainContainer">
    <header>
      <NuxtLink to="/">Мой профиль</NuxtLink>
      <NuxtLink to="/whyProgrammed">Почему программирование?</NuxtLink>
      <NuxtLink to="/interestingCSS">Интересный CSS</NuxtLink>
    </header>
    <slot />
    <footer>
      <NuxtLink to="https://github.com/madaoHas/aboutMe">Ссылка на GitHub</NuxtLink>
    </footer>
  </div>
</template>

<style scoped>
template {
  display: flex;
  flex-direction: column;
  min-height: 100%;
}
header {
  display: flex;
  gap: 20px;
  /*justify-content: space-between;*/
  border-bottom: solid gray;
  background-color: #1B1B1B;
  padding: 20px 20px 20px 150px;
}
header a {
  text-decoration: none;
  color: whitesmoke;
  font-family: Gill Sans;
}
header a:hover {
  color: gray;
}

footer {
  font-family: Gill Sans;
  position: fixed;
  bottom: 10px;
  right: 10px;
  background-color: #1B1B1B;
  padding: 10px;
}
footer a {
  color: whitesmoke;
  text-decoration: none;
}

@media (min-width: 320px) and (max-width: 768px) {
  header {
    gap: 10px;
    padding: 10px 10px 10px 10px;
    font-size: 14px;
  }
}
</style>