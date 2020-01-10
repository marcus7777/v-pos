<template>
  <div class="keyboard">
    <div class="grid">
      <md-button v-for="(v,k) in cat" :key="k" >{{v}}</md-button>
      <div class="pad">
        <div class="line" v-for="(line, j) in pad" :key="j" >
          <md-button v-for="(v,k) in line" :key="k" >{{v}}</md-button>
        </div>
      </div>
    </div>   
  </div>
</template>

<script>
  export default {
    name: "v-pos",
    components: {
    },
    methods: {
      press(key) {
      }
    },
    data(){
      return {
	cat:["a","b","c"],
	pad:[
          ["1","2","3"],
          ["4","5","6"],
          ["7","8","9"],
          [".","0","<"],
        ],
      }
    },
  }
</script>
