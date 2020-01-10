<template>
   <div class="keyboard">
     <NumericKeyboard layout="tel" @press="press" />
   </div>
</template>

<script>
  import { NumericKeyboard } from 'numeric-keyboard'
  export default {
    name: "v-pos"
    components: {
      NumericKeyboard
    },
    methods: {
      press(key) {
      }
    }
  }
</script>
