<template>
  <div class="columnas">
    <div class="b box1" v-on:click="color = 'red'"></div>
    <div id="box" :style="{background: color}"></div>
    <div class="b box2" @click="color = 'orange'"></div>
    <div class="b box3" @click="color = 'yellow'"></div>
    <div class="b box4" @click="color = 'green'"></div>
    <div class="b box5" 
    @click="color = 'rgb(52, 201, 221)'">
    </div>
    <div class="b box6" @click="box6"></div>
  </div>
</template>

<script>
export default {
  name: 'Cuadro',
  data() {
    return {
        color: 'red',
    }
  },
  
  methods: {
  box6: function (){
    this.color= 'rgb(187, 40, 118)'
	}
  }
}

</script>

<style scoped>
.columnas {
  display: grid;
  grid-template-columns: 50px 300px;
  grid-template-rows: 50px 50px 50px 50px 50px 50px;
}
#box {
  width: 300px;
  height: 300px;
  background-color: red;
  border: 1px solid black;
}
.b {
  width: 50px;
  grid-column: 1 / 2;
  height: 50px;
  border: 1px solid black;
}
.box1 {
  background-color: red;
}
.box2 {
    background-color:orange;
}
.box3 {
  background-color: yellow;
}
.box4 {
    background-color:green;
}
.box5 {
  background-color: rgb(52, 201, 221);
}
.box6 {
    background-color:rgb(187, 40, 118);
}
</style>
