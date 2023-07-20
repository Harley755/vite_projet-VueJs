<script>
import { ref } from 'vue'
import TheWelcome from '../components/TheWelcome.vue'

export default {
  components: { TheWelcome },

  setup() {
    let message = ref('Hello World')
    return {
      message
    }
  }
}
</script>

<template>
  <main>
    <TheWelcome />
    {{ message }}

    <input type="text" v-model="message" />
  </main>
</template>
