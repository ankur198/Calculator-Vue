<template>
  <div class="home">
    <Calculator class="calc" />
  </div>
</template>

<script>
// @ is an alias to /src
import Calculator from "./../components/Calculator/Calculator.vue";

export default {
  name: "home",
  components: {
    Calculator
  }
};
</script>
<style lang="scss" scoped>
.home {
  display: grid;
  align-items: center;
  justify-content: center;
  height: 100vh;
  .calc {
    height: 600px;
    width: 500px;
    border: solid 1px black;
  }
}
</style>
