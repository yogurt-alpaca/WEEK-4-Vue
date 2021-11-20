<template>
  <div>
    <h2>{{tittle}}</h2>
    <p>{{content}}</p>
  </div>
</template>

<script>
export default {
  name: "Text",
  props: {
      tittle: String,
      content: String,
  }
};
</script>

<style scoped>
div{
    display: flex;
    flex-direction: column;
    padding: 40px 12px;
}
h2{
    font-size: 34px;
    color: #fff;
    width: 735px;
    max-width: 0 0 12px;
    height: 38px;
}
p{
    font-size: 18px;
    color: #fff;
    width: 735px;
    height: 120px;
}
</style>