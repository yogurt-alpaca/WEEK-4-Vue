<template>
  <div class="nav">
    <a href="#" class="logo">
      <img src="../images/logo.png" alt="" />
    </a>
    <a href="#" class="microtext">
      <span>
        {{ microtext }}
      </span>
    </a>
    <ul>
      <li>
        <a href="#">{{ TextOne }}</a>
      </li>
      <li>
        <a href="#">{{ TextTwo }}</a>
      </li>
      <li>
        <a href="#">{{ TextThree }}</a>
      </li>
      <li>
        <a href="#">{{ TextFour }}</a>
      </li>
      <li>
        <a href="#">{{ TextFive }}</a>
      </li>
      <li>
        <a href="#">{{ TextSix }}</a>
      </li>
    </ul>
    <div class="list">
        <a href="#">
            {{all}}
        </a>
    </div>
    <div class="search">
        <a href="#">
            {{search}}
        </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Nav",
  data() {
    return {
      microtext: "Microsoft Edge Insider",
      TextOne: "下载",
      TextTwo: "最新动态",
      TextThree: "下一步",
      TextFour: "大型企业",
      TextFive: "社区",
      TextSix: "支持",
      all: "所有microsoft",
      search: "搜索",
    };
  },
};
</script>

<style scoped>
.nav {
  display: flex;
  width: 1304px;
  height: 54px;
  margin: 0 auto;
  padding: 0 70px;
  color: #f2f2f2;
  ;
}
.logo img {
  width: 108px;
  height: 23px;
  margin-top: 13.28px;
}
.microtext span {
  color: #f2f2f2;
  font-size: 18px;
  font-weight: 500;
  line-height: 53.14px;
  margin-left: 20px;
}
.microtext span:hover{
border-bottom: 2px solid #f2f2f2;
}
ul {
  display: flex;
  width: 800px;
}
ul li {
  float: left;
  margin-right: 20px;
}

ul li a{
    color: #f2f2f2;
    font-size: 13px;
}
ul li a:hover{
    border-bottom: 2px solid #f2f2f2;
}
.list{
    margin-right: 30px;
}
.list a{
    color: #f2f2f2;
    font-size: 13px;
    line-height: 54px;
}
.list a:hover{
    border-bottom: 2.5px solid #f2f2f2;
}
.search a{
    color: #f2f2f2;
    line-height: 54px;
    font-size: 13px;
}
.search a:hover {
    border-bottom: 2.5px solid #f2f2f2;
}
</style>>

