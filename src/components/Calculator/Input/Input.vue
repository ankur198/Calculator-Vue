<template>
  <div class="input">
    <Keypad></Keypad>
    <Operations></Operations>
  </div>
</template>

<script>
import Keypad from "./Keypad";
import Operations from "./Operations";
export default {
  name: "Input",
  components: {
    Keypad,
    Operations
  }
};
</script>

<style lang="scss" scoped>
.input {
  padding: 20px;
  border: 1px solid black;
}</style
>>
