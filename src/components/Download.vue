<template>
  <div class="download">
    <div class="download-body">
      <div class="left">
        <img
          id="left"
          src="https://daily.zhihu.com/img/new_home_v3/phone_sample.png"
          alt=""
          class="fadeInUp"
        />
      </div>
      <div class="right fadeInRight">
        <div class="right-top">
          <h1>每天三次&nbsp;&nbsp;每次七分钟</h1>
          <span>
            在中国，资讯类移动应用的人均阅读时长是5分钟，而在知乎日报，这个数字是21。
          </span>
        </div>
        <div class="right-bottom">
          <div class="right-bottom-l">
            <img
              src="https://daily.zhihu.com/img/new_home_v3/qr_top2.png"
              alt=""
            />
          </div>
          <div class="right-bottom-r">
            <div>
              <!-- <a href="">
                <img
                  src="https://daily.zhihu.com/img/new_home_v3/iphone_logo.png"
                  alt=""
                  id="img1"
                />
                iOS版</a
              > -->
              <el-button class="button1">
                <img
                  src="https://daily.zhihu.com/img/new_home_v3/iphone_logo.png"
                  alt=""
                  id="img1"
                />
                <span>iOS版</span>
              </el-button>
            </div>
            <div>
              <!-- <a href="">
                <img
                  src="https://daily.zhihu.com/img/new_home_v3/android_logo.png"
                  alt=""
                  id="img2"
                />
                Android版</a
              > -->

              <el-button class="button1">
                <img
                  src="https://daily.zhihu.com/img/new_home_v3/android_logo.png"
                  alt=""
                  id="img2"
                />
                <span>Android版</span>
              </el-button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Download",
};
</script>
<style scoped>
.download {
  background: #008bea;
  padding-top: 114px;
}
.download-body {
  width: 1460px;

  display: flex;
  margin: 0 auto;
}
.right-bottom {
  display: flex;
}

img#left {
  width: 615px;
  animation: fadeInUp 1s;
}
.left {
  margin: 20px 50px;
  margin-right: 152px;
  margin-bottom: -5px;
}
h1 {
  margin-top: 150px;
  font-size: 58px;
  color: #ffffff;
  font-weight: normal;
}
.right-top span {
  line-height: 40px;
  font-size: 24px;
  color: #99d1f8;
}
.right {
  padding-right: 55px;
  animation: fadeInRight 1s;
}
.right-bottom-l img {
  height: 220px;
  border-radius: 5px;
}
.right-bottom-r {
  margin-left: 75px;
}

.right-bottom {
  margin-top: 70px;
}
.right-bottom-r .button1 {
  /* display: block; */
  display: flex;
  height: 90px;
  width: 290px;
  line-height: 90px;
  /* background: #ffffff; */
  margin-bottom: 40px;
  border-radius: 5px;
  justify-content: center;
  font-size: 32px;
  /* color: #39442e; */
}
.right-bottom-r #img1 {
  margin-left: -83px;
  margin-right: 29px;
}
.right-bottom-r #img2 {
  margin-left: -42px;
  margin-right: 8px;
}
.right-bottom-r span {
  position: relative;
  top: -12px;
}
</style>