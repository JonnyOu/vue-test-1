<template>
  <div class="body">
    <el-carousel height="400px">
      <el-carousel-item v-for="item in items" :key="item.img">
        <img :src="item.img" alt />
      </el-carousel-item>
    </el-carousel>
    <Pagination class="pagination"/>
  </div>
</template>

<script>
import Pagination from "./pagination.vue";

export default {
  components: {
    Pagination
  },
  data() {
    return {
      items: [
        { url: "#abc", img: require("../../assets/img/banner-1.png") },
        { url: "#def", img: require("../../assets/img/banner-2.png") },
        { url: "#aaa", img: require("../../assets/img/banner-1.png") },
        { url: "#bbb", img: require("../../assets/img/banner-2.png") }
      ]
    };
  }
};
</script>

<style>

.pagination {
    margin-top: 30px;
}

.el-carousel__item img {
  width: 100%;
  height: 100%;
}

.el-carousel__item:nth-child(2n) {
  background-color: #99a9bf;
}

.el-carousel__item:nth-child(2n + 1) {
  background-color: #d3dce6;
}
</style>