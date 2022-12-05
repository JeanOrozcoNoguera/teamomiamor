<template>
  <div>
    <bienvenida/>
    <br> <br>
    <cartas/>
  </div>
</template>

<script>
import bienvenida from "@/components/Bienvenida";
import cartas from "@/components/Cartas";
export default {
  components: {
    bienvenida, cartas
  }
};
</script>
<style scoped>

.v-btn {
  text-transform: none !important;
}

</style>
