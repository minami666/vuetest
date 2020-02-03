<template>
  <div>
    <div v-if="isActive === false" v-on:click="aaa()" class="test">
      <div :class="{ hinge: aoao}" class="ddd">aaa</div>
      {{ msg }}
    </div>
    <div v-if="isActive === true" v-on:click="bbb()" class="testa">aaaaa</div>
  </div>
</template>

<style>
.test {
  width: 600px;
  height: 800px;
  background-color: aqua;
}
.testa {
  width: 600px;
  height: 800px;
  background-color: rgb(220, 9, 30);
}
.ddd{
  width: 100px;
  height: 100px;
  background-color: rgb(0, 0, 0);
}
</style>

<script>
export default {
  data() {
    return {
      msg: "アイウエお",
      isActive: false,
      hako: null,
      aoao: false
    };
  },
  methods: {
    aaa() {
      // this.isActive = true;
      this.aoao = true
    },
    bbb() {
      this.isActive = false;
    }
  }
};
</script>
