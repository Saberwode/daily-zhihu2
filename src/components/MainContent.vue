<template>
  <div class="content">
    <div class="maincontent">
      <div class="title">
        <span>浏览内容</span><span class="new">最新内容</span>
      </div>

      <div class="item">
        <div class="left">
          <content-item
            v-for="item in storiesLeft"
            :key="item.id"
            :url="item.url"
            :imgSrc="item.images[0]"
            :title="item.title"
          ></content-item>
        </div>
        <div class="center">
          <content-item
            v-for="item in storiesCenter"
            :key="item.id"
            :url="item.url"
            :imgSrc="item.images[0]"
            :title="item.title"
          ></content-item>
        </div>
        <div class="right">
          <content-item
            v-for="item in storiesRight"
            :key="item.id"
            :url="item.url"
            :imgSrc="item.images[0]"
            :title="item.title"
          ></content-item>
        </div>
      </div>
      <div class="more"><div>更多精彩可在知乎日报应用中查看</div></div>
      <div></div>
    </div>
  </div>
</template>
<script>
import axios from "axios";
import ContentItem from "@/components/ContentItem";
export default {
  name: "MainContent",
  data() {
    return {
      storiesLeft: [],
      storiesCenter: [],
      storiesRight: [],
    };
  },
  created() {
    // axios({
    //   url: "/api/3/stories/latest",
    // }).then((res) => {
    //   // console.log(res);
    //   this.storiesLeft = res.data.stories;
    //   console.log(this.stories);
    // });
    axios
      .all([
        axios({
          url: "/api/3/stories/latest",
        }),
        axios({
          url: "/api/3/news/before/20210710",
        }),
        axios({
          url: "/api/3/news/before/20210709",
        }),
      ])
      .then(
        axios.spread((res1, res2, res3) => {
          this.storiesLeft = res1.data.stories;
          this.storiesCenter = res2.data.stories;
          this.storiesRight = res3.data.stories;
        })
      );
  },
  components: {
    ContentItem,
  },
};
</script>
<style scoped>
.content {
  background: #f9f9f9;
}
.maincontent {
  width: 1460px;
  margin: 0 auto;
}
.item {
  display: flex;
  justify-content: space-around;
}
.left,
.center,
.right {
  margin: 20px;
}
.title {
  display: flex;
  justify-content: space-between;
}
.title span {
  font-size: 39px;
  height: 130px;
  line-height: 130px;
}
.new {
  color: #cccccc;
}
.more {
  display: flex;
  justify-content: center;
  height: 50px;
  line-height: 50px;
  padding-bottom: 135px;
}
.more div {
  display: block;
  background: #e8eef2;
  height: 92px;
  line-height: 92px;
  width: 1640px;
  text-align: center;
  font-size: 31px;
  border-radius: 5px;
  color: #15527b;
}
</style>