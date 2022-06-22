<template>
  <div style="padding: 10px">
    <el-row :gutter="20">
      <el-col :span="12">
        <el-card>
          <div style="padding: 10px 0; font-size: 18px">关于</div>
          <div class="demo-image">
            <div class="block" v-for="fit in fits" :key="fit">
              <span class="demonstration">{{ fit }}</span>
              <el-image
                style="width: 100px; height: 100px"
                :src="url"
                :fit="fit"></el-image>
            </div>
          </div>
        </el-card>
      </el-col>
    </el-row>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        fits: ['fill', 'contain', 'cover', 'none', 'scale-down'],
        url: 'http://www.tangzy.xyz/usr/uploads/2022/06/2730781865.jpg'
      }
    }
  }
</script>

<style scoped>

</style>
