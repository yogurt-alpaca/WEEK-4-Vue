<template>
  <div class="homeTop">
    <div class="textBox">
      <h1>查看即将推出的内容！</h1>
      <p>
        Microsoft Edge 预览频道现已推出移动版！
        请访问下载页面，根据你的移动设备选择要安装的版本。
        想成为第一批预览新增功能的人吗？ 我们将持续更新包含最新功能的 Insider
        Channels，请立即下载并加入 Microsoft Edge 预览体验成员社区。
      </p>
      <a href="#" class="download"><span>下载Beta渠道Windows10/11版</span></a>
      <a href="#" class="more">更多平台和渠道</a>
    </div>
    <img src="../images/homeTop.png" alt="" />
  </div>
</template>

<script>
export default {
  name: "homeTop",
};
</script>

<style scoped>
.homeTop {
  display: flex;
  justify-content: space-evenly;
  padding: 100px 0;
  width: 100%;
  height: 380px;

}
.textBox {
  width: 710px;
  height: 330px;
  text-align: center;
}
.textBox h1 {
  color: #fff;
  font-size: 54px;
  margin-top: 15px;
  margin-bottom: -15px;
}
.textBox p {
  font-size: 20px;
  color: #fff;
  margin-bottom: 40px;
}
.textBox .download span {
  display: inline-block;
  width: 312px;
  height: 66px;
  background-color: #0077d9;
  margin: 0 200px;
}
.textBox .download {
  font-size: 18px;
  color: #fff;
  line-height: 66px;

}

.textBox .download:hover{
  opacity: 0.8;
}
.textBox .more {
  display: inline-block;
  color: #70bfff;
  font-size: 15px;
  margin-top: 10px;
}
.textBox .more:hover{
  color: #b8dfff;
  border-bottom: 1px solid #b8dfff;
}
img {
  width: 593px;
  height: 294px;
}
</style>