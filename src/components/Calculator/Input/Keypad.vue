<template>
  <div class="keypad">
    <btn :name="i" :key="i" @click="addToNum" v-for="i in buttons"></btn>
  </div>
</template>

<script>
import btn from "./CalcBtn";
export default {
  name: "Keypad",
  data() {
    return {
      currentNum: "0",
      buttons: ["7", "8", "9", "4", "5", "6", "1", "2", "3", "0", "."]
    };
  },
  components: {
    btn
  },
  methods: {
    addToNum: function(val) {
      console.log(val);
      if (val === ".") {
        if (this.currentNum.includes(".") == false) {
          this.currentNum += ".";
        }
      } else if (this.currentNum == "0") {
        this.currentNum = val;
      } else {
        this.currentNum += val;
      }
      console.log(this.currentNum);
    }
  }
};
</script>

<style>
.keypad {
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
}
</style>
