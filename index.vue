<template>
  <div class="keyboard">
    <div class="grid">
      <md-button v-for="(v,k) in cat" :key="k" >{{v}}</md-button>
      <div class="pad md-layout-item md-size-66 md-small-size-100">
        <div class="line" v-for="(line, j) in pad" :key="j" >
          <md-button v-for="(v,k) in line" :key="k" >{{v}}</md-button>
        </div>
      </div>
    </div>   
  </div>
</template>
<style>
  .grid {
    grid-auto-columns: 6px;
    align-content: space-evenly;
    display: grid;
    grid-gap: 1rem;
    grid-template-columns: repeat(8, 1fr);
    grid-gap: 10px;
    grid-auto-rows: 100px;
    grid-template-areas:
      "o o o o o o o o"
      "c c c c c p p p"
      "c c c c c p p p"
      "c c c c c p p p";
  }
  .pad {
    grid-area: p;
  }
</style>
<script>
  export default {
    name: "v-pos",
    components: {
    },
    methods: {
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
