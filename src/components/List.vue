<template>
  <div class="footerList">
    <div class="header">{{ header }}</div>
    <ul>
      <li v-for="item in list" :key="item">{{ item.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "List",
  props: {
    header: String,
    list: Array,
  },
};
</script>

<style scoped>
.footerList{
  
  padding: 0 60px;
  color: #d0d0d0;
}
.header{
  padding: 36px 0 4px;
}
ul{
  margin: 0 0;
  padding: 0 0;
}
li{
font-size: 12px;
padding: 8px 0;
}
li a:hover{
  text-decoration-line: underline;
}
</style>