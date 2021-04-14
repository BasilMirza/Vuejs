<template>
  <pre id="hello">
      <input type="text" v-model="msg">
    {{ msg }}
    <b>{{ reversedMessage }}</b>
    A: <input type="number" v-model.lazy.number="a">
    B: <input type="number" v-model.lazy.number="b">

    <b>{{ computedProp }}</b>

</pre>
</template>
<script>
export default {
  name: "Hello World",

  data() {
    return {
      a: 200,
      b: 400,

      msg: "Hello, I am Basil.",
    };
  },
  computed: {
    computedProp: function() {
      return this.a / 2 + this.b / 2;
    },
    reversedMessage() {
      return this.msg
        .split("")
        .reverse()
        .join("");
    },
  },
  watch: {
    a: function() {
      alert("A value is changed");
    },
    computedProp: function() {
      alert("Computed value is now different");
    },
  },
};
</script>
