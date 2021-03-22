<template>
  <p>
    {{ string }}
  </p>
</template>

<script>
export default {
  name: "stringComp",
  data() {
    return {
      string: "入力された感想をここに出す"
    };
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped></style>
