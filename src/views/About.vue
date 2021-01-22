<template>
  <div class="about">
    <h1>This is an about page</h1>
    <hexagon-card></hexagon-card>
    <div>
      <glitch-button></glitch-button>
    </div>
  </div>
</template>

<script>
import GlitchButton from '../components/GlitchButton.vue'
import HexagonCard from '../components/HexagonCard'
export default {
components: {
  HexagonCard,
  GlitchButton
}

}
</script>
