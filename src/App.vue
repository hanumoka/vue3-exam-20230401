<template>
  <div class="name">하누모카 뷰3 예제 {{ name }}</div>
  <h1>aaaa</h1>
</template>

<script>
export default {
  setup() {
    const name = "hanumoka";

    return {
      name,
    };
  },
};
</script>

<style>
.name {
  color: red;
}
</style>
