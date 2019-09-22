<template>
  <div class="calcBtn" @click="clicked">
    {{ name }}
  </div>
</template>

<script>
export default {
  name: "CalcBtn",
  props: {
    name: String
  },
  methods: {
    clicked: function() {
      this.$emit("click", this.name);
    }
  }
};
</script>

<style>
.calcBtn {
  padding: 20px;
  margin: 10px;
  border: 1px solid black;
  text-align: center;
}
</style>
