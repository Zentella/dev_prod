<template>
  <div class="columnas">
    <div id="box1" v-on:click="box1"></div>
    <div
      id="box">
	</div>
    <div id="box2" v-on:click="box2"></div>
    <div id="box3" @click="box3"></div>
    <div id="box4" @click="box4"></div>
    <div id="box5" @click="box5"></div>
    <div id="box6" v-on:click="box6"></div>
  </div>
</template>

<script>
export default {
  name: 'Cuadro',  
  methods: {
	box1: function (){
		document
    .getElementById("box")
    .setAttribute("style", "width: 300px;height:300px;background-color: red;");
	},
	box2: function (){
		document
    .getElementById("box")
    .setAttribute(
      "style",
      "background: orange;"
    );
	},
  box3: function (){
		document
    .getElementById("box")
    .setAttribute("style", "width: 300px;height:300px;background-color: yellow;");
	},
  box4: function (){
		document
    .getElementById("box")
    .setAttribute("style", "width: 300px;height:300px;background-color: green;");
	},
  box5: function (){
		document
    .getElementById("box")
    .setAttribute("style", "width: 300px;height:300px;background-color: rgb(52, 201, 221);");
	},
  box6: function (){
		document
    .getElementById("box")
    .setAttribute("style", "width: 300px;height:300px;background-color: rgb(187, 40, 118);");
	},
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
#box1 {
  width: 50px;
  grid-column: 1 / 2;
  height: 50px;
  background-color: red;
  border: 1px solid black;
}
#box2 {
    width: 50px;
    grid-column: 1 / 2;
    height:50px;
    background-color:orange;
    border:1px solid black;
}
#box3 {
  width: 50px;
  grid-column: 1 / 2;
  height: 50px;
  background-color: yellow;
  border: 1px solid black;
}
#box4 {
    width: 50px;
    grid-column: 1 / 2;
    height:50px;
    background-color:green;
    border:1px solid black;
}
#box5 {
  width: 50px;
  grid-column: 1 / 2;
  height: 50px;
  background-color: rgb(52, 201, 221);
  border: 1px solid black;
}
#box6 {
    width: 50px;
    grid-column: 1 / 2;
    height:50px;
    background-color:rgb(187, 40, 118);
    border:1px solid black;
}
</style>
