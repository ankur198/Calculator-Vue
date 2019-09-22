<template>
  <div class="Calculator">
    <outputMy :ans="currentResult" class="output"></outputMy>
    <inputMy class="input"></inputMy>
  </div>
</template>

<script>
import InputMy from "./Input/Input";
import OutputMy from "./Output";
export default {
  name: "Calculator",
  data() {
    return {
      currentResult: 0
    };
  },
  components: {
    InputMy,
    OutputMy
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.Calculator {
  display: grid;
  padding: 10px;
  grid-gap: 10px;
}
</style>
