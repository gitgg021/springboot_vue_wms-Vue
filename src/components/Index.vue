<template>
  <el-container style="height: 100%; border: 1px solid #eee">
    <el-aside width="200px" style="background-color: rgb(238, 241, 246);height: 100%">
      <AsidePage></AsidePage>
    </el-aside>

    <el-container style="height: 100%;">
      <el-header style="text-align: right; font-size: 12px;height: 100%;border-bottom: rgba(30,0,0,0.66) 1px solid;">
       <HeaderPage></HeaderPage>
      </el-header>

      <el-main style="height: 100%;">
          <MainPage></MainPage>
      </el-main>
    </el-container>
  </el-container>

</template>

<script>



import AsidePage from "./Aside"
import HeaderPage from "./Header"
import MainPage from "./Main"

export default {
  name: "IndexPage",
  components: {AsidePage,HeaderPage,MainPage},
  }
</script>

<style scoped>
.el-header {
  #background-color: #B3C0D1;
  color: #333;
  line-height: 60px;
}
.el-main{
  padding: 5px;
}

.el-aside {
  color: #333;
}
</style>