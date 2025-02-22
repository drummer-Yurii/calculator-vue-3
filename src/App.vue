<script setup>
import { ref } from "vue";

const display = ref('');
const buttons = [
  { value: 'AC', type: 'clear' },
  { value: 'DEL', type: 'delete' },
  { value: '.', type: 'operator' },
  { value: '/', type: 'operator' },

  { value: '7' },
  { value: '8' },
  { value: '9' },
  { value: '*', type: 'operator' },

  { value: '4' },
  { value: '5' },
  { value: '6' },
  { value: '-', type: 'operator' },

  { value: '1' },
  { value: '2' },
  { value: '3' },
  { value: '+', type: 'operator' },

  { value: '000' },
  { value: '00' },
  { value: '0' },
  { value: '=', type: 'equals' },
];
</script>

<template>
  <div class="calculator">
    <input type="text" v-model="display" class="display" disabled />
    <div class="button"></div>
  </div>
</template>
