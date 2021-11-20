<template>
  <div class="homeMiddle">
    <div class="mobile">
      <div class="mobileBox">
        <div class="mobileImg"><img src="../images/mobile.png" alt="" /></div>
        <div class="mobileText">
          <p class="yellow">现已推出</p>
          <h2>加入Microsoft Edge移动版预览体验计划</h2>
          <a href="#">更多移动版频道</a>
        </div>
      </div>
      <div class="mobileSystem">
        <div class="mobileAndroid">
          <img src="../images/AndroidLogo.png" alt="" class="androidLogo" />
          <h3>Android版 Beta频道</h3>
          <img src="../images/qr.png" alt="" class="qr" />
          <a href="#" class="GooglePlay"
            ><img src="../images/GooglePlay.png" alt="" class="googleplay"
          /></a>
        </div>
        <div class="mobileIos">
          <img src="../images/iosLogo.png" alt="" class="iosLogoImg" />
          <h3>iOS 版 Insider Channels</h3>
          <p>当前向新用户开放</p>
          <a href="#" class="downloadIos">
            <span class="blue">下载Beta渠道iOS版</span>
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "homeMiddle",
};
</script>


<style>
.homeMiddle {
  width: 100%;
  background-color: #181818;
  height: 379px;
  padding: 30px 0;
}
.homeMiddle .mobile {
  display: flex;
  justify-content: center;
  width: 100%;
  padding: 50px 0;
}
.homeMiddle .mobileBox{
  display: flex;
}
.homeMiddle .mobileImg {
  display: inline-block;
  width: 152px;
  height: 233px;
  margin-right: 20px;
  margin-top: 30px;
}
.homeMiddle .mobileImg img {
  width: 160px;
  height: 250px;
}

.homeMiddle .mobileText {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  padding: 0 24px;
}
.homeMiddle .mobileText .yellow{
  width: 72px;
  height: 24px;
  line-height: 24px;
  text-align: center;
  font-size: 12px;
  color: #262626;
  font-weight: 700;
  background: #fdb814;
}
.homeMiddle .mobileText h2{
  font-size: 28px;
  font-weight: normal;
  width: 400px;
}
.homeMiddle .mobileText a{
  font-size: 15px;
  color: #70bfff;
  text-decoration-line: underline;
}
.homeMiddle .mobileText a:hover{
  color: #b8dff1;
}
.homeMiddle .mobileSystem{
  display: flex;
  justify-content: space-around;
  width: 550px;
}
.homeMiddle .mobileAndroid {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
  height: 290px;
  padding: 12px 0;
  margin: 0 30px;
}

.mobile .mobileAndroid .androidLogo {
  width: 36px;
  height: 36px;
}
.mobile .mobileAndroid h3 {
  font-size: 18px;
}
.mobile .mobileAndroid .qr {
  width: 124px;
  height: 124px;
}
.mobile .mobileAndroid .googleplay {
  width: 132px;
  height: 40px;
}
.mobile .mobileIos{
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: first baseline;
  padding: 12px 0;
}
.mobile .mobileIos .iosLogoImg{
  width: 36px;
  height: 36px;
}
.mobile .mobileIos .blue{
  display: inline-block;
  background-color: #0267b8;
  padding: 12px 36px;
  font-size: 18px;
}
.mobile .mobileIos .blue:hover{
  opacity: 0.7;
}

</style>