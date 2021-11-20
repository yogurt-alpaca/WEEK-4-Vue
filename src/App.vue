<template>
  <div class="h">
    <div class="nav">
      <Nav></Nav>
    </div>
    <div class="homeTop">
      <home-top></home-top>
    </div>
    <home-middle></home-middle>
    <div class="TextImg">
      <div class="TextImgBox">
        <Text :tittle="experienceTittle" :content="experienceContent"></Text>
        <div class="IMGBOX">
          <img :src="experienceImgPath" alt="" class="IMG" />
        </div>
      </div>
      <div class="TextImgBox">
        <div class="IMGBOX">
          <img src="./images/people.png" alt="" class="IMG" />
        </div>
        <Text :tittle="peopleTittle" :content="peopleContent"></Text>
      </div>
      <div class="TextImgBox">
        <Text :tittle="checkTittle" :content="checkContent"></Text>
        <div class="IMGBOX">
          <img src="./images/check.png" alt="" class="IMG" />
        </div>
      </div>
      <div class="TextImgBox">
        <div class="IMGBOX">
          <img src="./images/listen.png" alt="" class="IMG" />
        </div>
        <Text :tittle="listenTittle" :content="listenContent"></Text>
      </div>
    </div>
    <div class="ListBox">
      <List :header="listHeader1" :list="footList1"></List>
      <List :header="listHeader2" :list="footList2"></List>
      <List :header="listHeader3" :list="footList3"></List>
      <List :header="listHeader4" :list="footList4"></List>
      <List :header="listHeader5" :list="footList5"></List>
      <List :header="listHeader6" :list="footList6"></List>
    </div>
    <div class="homeBottom">
      <home-bottom :language="Language" :list="bottomList"></home-bottom>
    </div>
  </div>
</template>
<script>
import Nav from "./components/nav.vue";
import homeTop from "./components/homeTop.vue";
import homeMiddle from "./components/homeMiddle.vue";
import Text from "./components/Text.vue";
import List from "./components/List.vue";
import homeBottom from "./components/homeBottom.vue";
export default {
  components: {
    Nav,
    homeTop,
    homeMiddle,
    Text,
    List,
    homeBottom,
  },
  data() {
    return {
      experienceTittle: "成为 Microsoft Edge 预览体验成员",
      experienceContent:
        "我们的预览体验成员社区在帮助构建 Microsoft Edge 方面发挥了重大作用，而且我们的创新从未停止。 如果你想要了解我们的后续工作，我们诚邀你下载我们的预览渠道并加入预览体验成员社区。 届时你将可以抢先预览新功能，并且有机会在开发过程中与 Microsoft Edge 团队合作。 你的反馈和想法可以帮助我们改进，因此我们希望你能加入我们。 单击下载以开始使用！",
      experienceImgPath: require("./images/experience.png"),
      peopleTittle: "为大众打造更好的互联网空间",
      peopleContent:
        "我们在 Microsoft Edge 的开发过程中采用了 Chromium 开源项目，以此来为我们的客户提供更好的网站兼容性，并为所有的网站开发人员降低网站的碎片化程度。 我们将继续为 Chromium 项目做出积极贡献。 到目前为止，我们已经兑现了 1,700 多项承诺，并期待继续积极参与社区互动，为大众打造更好的互联网空间。 如需详细了解我们的贡献，请参阅 GitHub 上的 Microsoft Edge “Explainers”，并查看我们的源代码发布。",
      checkTittle: "查看 Microsoft Edge Insider Channels",
      checkContent:
        "我们提供三个预览渠道：Beta、Dev 和 Canary。 这些频道适用于所有受支持版本的 Windows、Windows Server 以及 macOS。 Beta 版频道可以提供最稳定的预览版体验，每 4 周更新一次。 开发频道每周更新一次，稳定性略逊于 Beta 版，但优于 Canary。 对于想要在相对稳定的版本内获取最新更新的人员，Dev 是一个不错的选择。 如果你想要查看我们昨天的工作并获取每日更新，那么 Canary 可能是你的理想预览渠道。 安装预览渠道不需要卸载 Microsoft Edge 的已发布版本，你可以同时安装多个版本。 若要详细了解不同的渠道并开始使用，请转到 下载页。",
      listenTittle: "我们乐于倾听！",
      listenContent:
        "Microsoft Edge 团队希望倾听你的声音。 在使用预览渠道时，请务必通过工具栏上的“发送反馈”按钮来分享你的反馈。 你还可以访问我们的 Microsoft Edge 预览体验成员论坛或在 Twitter 上关注 @MSEdgeDev。 我们会定期分享来自预览体验成员社区的热门反馈总结，以便你可以了解最受期待的功能、最新出现的问题以及你的反馈对产品产生的影响。 衷心希望你加入社区。如果尚未加入，我们期待倾听你的想法！",

      listHeader1: "新增内容",
      footList1: [
        { name: "Microsoft 365" },
        { name: "Surface Laptop 2" },
        { name: "Surface Go" },
        { name: "Windows 11 应用程序" },
      ],

      listHeader2: "Microsoft Store",
      footList2: [
        { name: "帐户个人资料" },
        { name: "下载中心" },
        { name: "订单跟踪" },
      ],

      listHeader3: "教育",
      footList3: [
        { name: "Microsoft 教育领域" },
        { name: "适合学生的 Office" },
        { name: "适用于学校的 Office 365" },
        { name: "Microsoft Azure 教育领域" },
      ],

      listHeader4: "企业",
      footList4: [
        { name: "Azure" },
        { name: "AppSource" },
        { name: "汽车" },
        { name: "政府机构" },
        { name: "医疗保健" },
        { name: "制造业" },
        { name: "金融服务" },
        { name: "零售业" },
      ],

      listHeader5: "开发人员",
      footList5: [
        { name: "Microsoft Visual Studio" },
        { name: "Windows 开发人员中心" },
        { name: "开发人员中心" },
        { name: "Microsoft 开发人员计划" },
        { name: "第9频道" },
        { name: "Microsoft 365 开发人员中心" },
        { name: "Microsoft 365 开发人员计划" },
      ],

      listHeader6: "公司",
      footList6: [
        { name: "招贤纳士" },
        { name: "关于 Microsoft" },
        { name: "公司新闻" },
        { name: "Microsoft 隐私" },
        { name: "投资人" },
        { name: "安全性" },
      ],
      Language: "中文（中国）",
      bottomList: [
        { name: "与 Microsoft联系" },
        { name: "隐私" },
        { name: "使用条款" },
        { name: "商标" },
        { name: "关于我们的广告" },
        { name: "京ICP备09042378号-6" },
        { name: "京公网安备 11010802023178" },
        { name: " © Microsoft 2021" },
      ],
    };
  },
};
</script>
<style>
body {
  margin: 0 0;
  padding: 0 0;
}
.h {
  margin: 0 auto;
  padding: 0 0;
  width: 100%;
  color: #fff;
}
a {
  text-decoration: none;
  color: #fff;
}
li {
  list-style: none;
}
.nav {
  background-color: #000;
}
.homeTop{
   background-color: #242424
}
.TextImg {
  background-color: #303030;
}
.TextImg .TextImgBox{
  display: flex;
  justify-content: space-evenly;
  padding: 24px 0;
}
.TextImg div .IMGBOX {
  width: 455px;
  height: 260px;
}
.TextImg div .IMG {
  width: 455px;
  height: 260px;
}

.ListBox {
  display: flex;
  justify-content: center;
  background-color: #181818;
}
.homeBottom{
  width:100%;
  background-color: #181818;
}
</style>
