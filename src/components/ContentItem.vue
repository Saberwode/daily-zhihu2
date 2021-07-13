<template>
  <div class="item">
    <div class="contentitem">
      <a :href="url">
        <img :src="imgSrc" alt="" />
        <span>{{ title }}</span>
      </a>
    </div>
  </div>
</template>
<script>
export default {
  name: "ContentItem",

  props: {
    title: String,
    url: String,
    imgSrc: String,
  },
};
</script>
<style scoped>
.item {
  padding: 30px;
  display: flex;
  justify-content: center;
  padding: 30px;
  background: #ffffff;
  margin-bottom: 30px;
  border-radius: 5px;
}
.contentitem {
  width: 399px;
  /* padding: 10px; */

  display: flex;
  justify-content: center;
}
img {
  display: block;
  max-width: 100%;
  height: 390px;
  margin-bottom: 1em;
}
.contentitem a span {
  font-size: 24px;
  line-height: 40px;
}
</style>