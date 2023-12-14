<template>
  <label>Your Password here :</label>
  <input :type="type_input" /> <br /> <br /> <br /> 
  <button @click="switchf"  style="padding: 15px;color: green; background-color: beige ; border: 1px solid rgb(153, 137, 137);"  >
    SHOW/HIDE YOUR PASSWORD
  </button>
</template>
<script>
export default {
  data: function () {
    return {
      type_input: "text",
    };
  },
  methods: {
    switchf() {
      this.type_input == "password" ? (this.type_input = "text") : (this.type_input = "password");
    },
  },
};
</script>
