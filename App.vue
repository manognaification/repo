<template>
  <div class="container">
    <h1>Hello, my name is {{ name }}.</h1>

    <p class="description">
      {{ about }}
    </p>

    <p class="date-today">Today's date is: <strong>{{ todayDate }}</strong></p>

    <div class="class-feedback">
      <h2>How I felt about today's classes:</h2>
      <textarea
        v-model="classFeeling"
        placeholder="Class is very excellent,"
        rows="5"
      ></textarea>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'


const name = ref('Manogna')


const about = ref('I am a passionate Vue.js developer learning new frontend technologies every day.')


const todayDate = ref(new Date().toLocaleDateString())


const classFeeling = ref('')
</script>


