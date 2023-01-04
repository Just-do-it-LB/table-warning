<template>
  <div>
    <h1>The opacity property</h1>
    <div id="myDIV">
      <div id="div2">A yellow DIV element.</div>
      <div id="div1">Change the opacity of the blue DIV.</div>
    </div>
  </div>
</template>

<script></script>

<style>
body {
  background-color: #e7e9eb;
}
#myDIV {
  height: 300px;
  background-color: #ff0f0f;
}
#div2 {
  border: 1px solid black;
  background-color: yellow;
  width: 200px;
  height: 100px;
  position: relative;
  top: 80px;
  left: 20px;
  padding: 20px;
}
#div1 {
  border: 1px solid black;
  position: relative;
  left: 50px;
  padding: 20px;
  background-color: lightblue;
  width: 200px;
  height: 100px;
  opacity: 0.4;
}
</style>
