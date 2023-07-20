<script>
import flash from '@/mixins/flash.js'

export default {
  mixins: [flash]
}
</script>


<template>
  <div class="about">
    <button @click="flash('It works')">Click Me</button>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
