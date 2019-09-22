<template>
  <div class="output">{{ ans }}</div>
</template>

<script>
export default {
  name: "Output",
  props: {
    ans: Number
  }
};
</script>

<style lang="scss" scoped>
.output {
  border: 1px solid black;
  padding: 20px;
  display: grid;
  align-content: flex-end;
  justify-content: flex-end;
}
</style>
