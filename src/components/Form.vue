<template>
  <div class="form">
      <h1>{{ msg }} </h1>
  </div>
</template>

<script>
export default {
    name: "Form",
    data: function(){
        return {
            msg: "Form page"
        }
    },
}
</script>

<style>
.active{
    color: red;
}
</style>