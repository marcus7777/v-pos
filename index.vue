<template>
  <div class="keyboard">
    <div class="grid">
      <div v-for="(v,k) in cat" :key="k" >{{v}}</div>
      <div class="gridb">
        <div>1</div>
        <div>2</div>
        <div>3</div>
        <div>4</div>
        <div>5</div>
        <div>6</div>
        <div>7</div>
        <div>8</div>
        <div>9</div>
        <div>0</div>
        <div>.</div>
        <div><</div>
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
	cat:["a","b","c"]
      }
    },
  }
</script>
