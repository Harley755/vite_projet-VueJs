<script setup>
import { ref, watch } from 'vue'
import { useStorage } from '@/composables/useStorage.js'

let food = useStorage('food')

// let food = ref(localStorage.getItem('food'))
// let age = ref(localStorage.getItem('age'))

// watch(food, (val) => {
//   write('food', val)
// })

// watch(age, (val) => {
//   write('age', val)
// })

// setTimeout(() => {
//   food.value = 'changed !'
// }, 2000)
</script>


<template>
  <div class="about">
    <p>What is ur favorite food ?</p>
    <input type="text" v-model="food" />
    <p>How old are u</p>
    <input type="number" v-model="age" />
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
