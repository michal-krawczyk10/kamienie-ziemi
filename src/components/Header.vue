<template>
  <header class="header">
    <button class="btn__head">
      <router-link to="/">Home</router-link>
    </button>
    <span class="header__span">|</span>
    <button class="btn__head">
      <router-link to="/about">About</router-link>
    </button>
    <span  class="header__span">|</span>
    <button class="btn__head">
      <router-link to="/pageone">Page One</router-link>
    </button>
    <span class="header__span">|</span>
    <button class="btn__head">
      <router-link to="/pagetwo">Page Two</router-link>
    </button>
  </header>
</template>
<style lang="scss">
.header {
  display: flex;
  justify-content: flex-end;
  &__span {
    padding: 0.5rem;
  }
}
.btn {
  &__head {
    
  }
}
</style>