<script>
import { useFlash } from '@/composables/useFlash.js'

export default {
  setup() {
    let { flash } = useFlash()

    return { flash }
  }
}
</script>

<template>
  <main>
    <p>
      <button @click="flash('Success !', 'It works')">Click Me</button>
    </p>
  </main>
</template>
