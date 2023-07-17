<template>
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <footer>
      <div>
        <Boat />
      </div>
    <Waves />
  </footer>
</template>
<script>
import Boat from '../components/Boat.vue';
import Waves from '@/components/Waves.vue';
export default {
  components: {
    Waves, Boat
  }
}
</script>
<style>
body {
  height: 100%;
  overflow: hidden;
}
footer div {
 position: absolute;
}
</style>