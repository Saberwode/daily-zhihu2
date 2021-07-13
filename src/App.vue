<template>
  <div id="app">
    <el-backtop
      target=".page-component__scroll .el-scrollbar__wrap"
    ></el-backtop>
    <Header></Header>
    <Download></Download>
    <MainContent></MainContent>
    <Footer></Footer>
  </div>
</template>
<script>
import Header from "@/components/Header";
import Download from "@/components/Download";
import MainContent from "@/components/MainContent";
import Footer from "@/components/Footer";
export default {
  name: "App",
  components: {
    Header,
    Download,
    MainContent,
    Footer,
  },
};
</script>
<style>
@import url("assets/css/main.css");
</style>
