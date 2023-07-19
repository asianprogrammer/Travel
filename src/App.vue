<script setup>
import SliderUI from './components/SliderUI.vue';
import NaveUI from "./components/NaveUI.vue";
</script>
<template>
  <section>
    <div>
      <SliderUI />
    </div>
    <div class="NaveUI">
      <NaveUI />
    </div>
  </section>
</template>
<style scoped>
.NaveUI {
  top: 20px;
  right: 20px;
  width: 700px;
  height: 100vh;
  padding: 40px;
  background: #fff;
  position: absolute;
  border-radius: 12px;
}
</style>