<template>
  <div class="mainheader">
    <div class="header">
      <img src="https://daily.zhihu.com/img/new_home_v3/top_logo.png" alt="" />
      <div>
        <span><a href="">浏览内容</a></span>
        <span><a href="" class="active">App下载</a></span>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: "Header",
};
</script>
<style scoped>
.mainheader {
  /* 固定header */
  position: fixed;
  background: #ffffff;
  width: 100%;
}
.header {
  width: 1460px;
  margin: 0 auto;
  height: 114px;
  line-height: 114px;
  display: flex;
  /* 垂直居中 */
  align-items: center;
  /* 两边对齐 */
  justify-content: space-between;
}
img {
  float: left;
  height: 75px;
}
span {
  float: right;
  width: 185px;
  display: flex;
  justify-content: center;
  line-height: 32px;
}
span a {
  font-size: 24px;
  /* background: #f0f9ff; */
  padding: 11px 44px;
}
span a.active {
  background: #f0f9ff;
  border-radius: 5px;
  color: #008bed;
}
</style>