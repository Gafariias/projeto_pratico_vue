<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <HelloI18n/>,
  <LocaleSwitcher/>
</template>

<script>
import HelloI18n from './components/HelloI18n.vue'
import LocaleSwitcher from './components/LocaleSwitcher.vue'

export default {
  name: 'App',
  components: {
    HelloI18n,
    LocaleSwitcher
  }
}
</script>
