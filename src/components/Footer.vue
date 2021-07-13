<template>
  <div class="footer">
    <div class="mainfooter">
      <div class="left">
        <p>
          知乎日报是一款拥有千万用户的资讯类客户端，每日提供来自知乎社区的精选问答，还有国内一流媒体的专栏特稿。
        </p>
        <p>
          主题日报包括动漫、设计、大公司、游戏、财经、电影、电子音乐、互联网安全等丰富内容，为业内人和资深爱好
          者推荐各领域最精彩文章，满足高质量阅读需求。
        </p>
        <p>在知乎日报，告别浮躁，重获阅读的愉悦。</p>
        <p>京 ICP 证 110745 号</p>
        <p>
          <img
            src="https://pic3.zhimg.com/80/v2-d0289dc0a46fc5b15b3363ffa78cf6c7.png"
            alt=""
          />
          <a
            href="http://www.beian.gov.cn/portal/registerSystemInfo?recordcode=11010802020088"
          >
            京公网安备 11010802010035 号
          </a>
        </p>
        <p>©zhihu 2015</p>
      </div>
      <div class="right">
        <img
          src="https://daily.zhihu.com/img/new_home_v3/qr_bottom.png"
          alt=""
        />
        <p>扫描下载客户端</p>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Footer",
};
</script>
<style scoped>
.footer {
  background: #e5e5e5;
}
.mainfooter {
  display: flex;
  width: 1460px;
  padding-top: 50px;
  margin: 0 auto;
  font-size: 21px;
}
p {
  margin-bottom: 31px;
  color: #666666;
}
.left {
  width: 1076px;
  margin-right: 150px;
}

.right img {
  height: 220px;
  background: #ffffff;
  padding: 10px;
  border-radius: 5px;
}
.right p {
  text-align: center;
  font-size: 24px;
  margin-top: 10px;
}
</style>