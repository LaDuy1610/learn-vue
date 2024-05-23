<template>
  <div>
    <p>Giá trị A: {{ tangA }}</p>
    <p>Giá trị B: {{ tangB }}</p>
    <button @click="a++">Cộng A</button>
    <button @click="b++">Cộng B</button>

    <div>
      <p>Hiện hay ẩn?</p>
      <p v-if="logic">Hiện</p>
      <button @click="logic = !logic">Đổi</button>
    </div>
  </div>
</template>

<style></style>

<script>
export default {
  data() {
    return {
      a: 0,
      b: 0,
      logic: true,
    };
  },
  computed: {
    tangA() {
      console.log("goi A");
      return this.a;
    },
    tangB() {
      console.log("goi B");
      return this.b;
    },
  },
  methods: {},
};
</script>
