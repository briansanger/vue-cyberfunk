<template>
  <div class="about">
    <h1>This is an about page</h1>
    <hexagon-card></hexagon-card>
    <div>
      <glitch-button></glitch-button>
    </div>
    <div>
      <circuit-pattern></circuit-pattern>
    </div>
  </div>
</template>

<script>
import GlitchButton from '../components/GlitchButton.vue';
import HexagonCard from '../components/HexagonCard';
import CircuitPattern from '@/components/CircuitPattern';

export default {
components: {
  HexagonCard,
  GlitchButton,
  CircuitPattern
}

}
</script>
