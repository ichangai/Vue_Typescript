<script setup lang="ts">
import { reactive, ref } from 'vue';

const state = reactive({
  name: 'Jackson',
  age: 24
})

// state.name = 9;

let first_name = ref<string>()
let age = ref<number>()


first_name.value = 'joe'
age.value = 39
</script>

<template>
  <div>
    <div class="app">
      hello, {{ state.name }} <br>
        Welcom, {{ first_name }} <br>
          age, {{ age }}
    </div>
  </div>
</template>

<style scoped></style>
