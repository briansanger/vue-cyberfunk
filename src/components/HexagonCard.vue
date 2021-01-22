<template>
  <div class="hexagon"><span>POOOOO</span></div>
</template>

<script>
export default {};
</script>

<style scoped>
.hexagon {
  position: relative;
  width: 300px;
  height: 173.21px;
  background-color: #8f8f8f;
  margin: 86.6px 0;
  box-shadow: 0 0 50px rgba(255, 0, 0, 1);
}

.hexagon:before,
.hexagon:after {
  content: "";
  position: absolute;
  z-index: 1;
  width: 212.13px;
  height: 212.13px;
  -webkit-transform: scaleY(0.5774) rotate(-45deg);
  -ms-transform: scaleY(0.5774) rotate(-45deg);
  transform: scaleY(0.5774) rotate(-45deg);
  background-color: inherit;
  left: 43.934px;
  box-shadow: 0 0 50px rgba(255, 0, 0, 1);
}

.hexagon:before {
  top: -106.066px;
}

.hexagon:after {
  bottom: -106.066px;
}

/*cover up extra shadows*/
.hexagon span {
  display: block;
  position: absolute;
  top: 0px;
  left: 0;
  width: 300px;
  height: 173.2051px;
  z-index: 2;
  background: inherit;
}
</style>
