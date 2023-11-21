<script setup>
  import Hello from './components/Hello.vue';
  import Skill from './components/Skill.vue';
  import Experience from './components/Experience.vue';
</script>

<template>
  <header class="header__background h-screen">
    <div class="block lg:flex justify-between">
      <Hello class="lg:w-1/4 w-full"/>
      <div class="w-1/3">
        <Skill />
        <Experience />
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
.header {
  &__background {
    background: linear-gradient(to top, rgba(134, 134, 134, 0.7) 0%,rgba(57, 57, 57, 0.7) 100%), url('./assets/bg.jpg');
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
  }
}
</style>