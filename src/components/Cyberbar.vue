<template>
  <div class="ui">
    <nav class="scene_nav">
      <ol class="scene_nav_list">
        <li
          class="scene_nav_item"
          v-for="(params, index) in maxScene"
          :key="index"
        >
          <button
            class="scene_nav_button"
            @click="scene = index"
            :class="{ 'o-active': scene === index }"
          ></button>
        </li>
      </ol>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      scene: 0,
      maxScene: 10,
    };
  },
};
</script>

<style scoped>
body {
  display: flex;
  justify-content: center;
  align-items: center;
  /* width: 100vw;
  height: 100vh; */
  overflow: hidden;
  background: radial-gradient(ellipse at bottom, #1b2735 0%, #090a0f 100%);
}

.scene_nav {
  position: relative;
}
.scene_nav_list {
  display: flex;
  margin: 0;
  padding: 0;
  transform: scaleY(0.6);
}
.scene_nav_item {
  display: block;
}
.scene_nav_item:nth-child(even) {
  transform: scaleY(-1);
}
.scene_nav_item:not(:first-child) {
  margin-left: -40px;
}
.scene_nav_button {
  display: block;
  width: 100px;
  height: 100px;
  margin: 0;
  padding: 0;
  border: none;
  background: #0a7896;
  outline: none;
  cursor: pointer;
  transition: 500ms;
  -webkit-clip-path: polygon(50px 0, calc(100% - 50px) 0, 100% 100%, 0 100%);
  clip-path: polygon(50px 0, calc(100% - 50px) 0, 100% 100%, 0 100%);
}
.scene_nav_button.o-active {
  width: 300px;
  background: #64fafa;
}
.scene_nav_button:hover {
  background: #64fafa;
}
</style>
