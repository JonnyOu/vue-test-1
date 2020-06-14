<template>
  <div class="header">
    <div class="img">
        <img src="https://s0.meituan.net/bs/fe-web-meituan/fa5f0f0/img/logo.png" alt="">
    </div>
    <div class="nav">
        <el-row>
            <el-col :span="6" style="text-align:right"><a href="">天工开物</a> </el-col>
            <el-col :span="6" style="text-align:right"><a href="">本草纲目</a></el-col>
            <el-col :span="6" style="text-align:right"><a href="">三国演义</a></el-col>
            <el-col :span="6" style="text-align:right"><a href="">资治通鉴</a></el-col>
        </el-row>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
.header {
    position: relative;
}
.img {
    float: left;
    width: 30%;
    /* background-color: wheat; */
}
.nav {
    width: 40%;
    /* background-color: violet; */
    float: right;
    margin: auto auto;
    top: 50%;
    position: absolute;
    right: 0%;
    top: 30%;
}

a {
    text-decoration: none;
}





</style>