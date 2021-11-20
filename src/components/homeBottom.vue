<template>
  <div>
    <span>
      <a href="#"><img src="../images/earth.png" />{{ language }}</a>
    </span>
    <ul>
      <li v-for="item in list" :key="item">{{ item.name }}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "homeBottom",
  props: {
    language: String,
    list: Array,
  },

};
</script>

<style scoped>
div{
  width: 1300px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  padding: 20px 70px;

}
img{
  width: 20px;
  height: 20px;
  padding-right: 4px;
}
span a{
  line-height: 47px;
  font-size: 12px;
}
ul{
  display: flex;
  flex-direction: row;
}
ul li{
  font-size: 12px;
  padding: 0 10px;
}
</style>