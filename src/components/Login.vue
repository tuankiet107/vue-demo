<template>
  <div class="login">
    <label for="">Vui lòng nhập tên</label>
    <br>
    <input type="text" >
    <button @click="handleSubmit">Submit</button>
  </div>
</template>

<script>
export default {
  name: "login",
  data: function() {
  return {
      msg: "Welcome to Login page"
    };
  },
  methods: {
    handleSubmit(){
      this.$router.push("/")
    }
  }
};
</script>

<style scoped>
.login{
  margin-top: 30px;
}
label{
  margin-right: 5px;
}
</style>
