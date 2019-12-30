<template>
  <view class="list">
  <view  @click="goDetail(item.id)"  v-for="(item,index) in heroList" :key = "index">
    <image :src="item.iconUrl"></image>
    <text class="name">{{item.name}}</text>
  </view>
</view>
</template>

<script>
import heroList from '../../data/lol_duowan'
export default {
  data () {
    return {
      heroList
    }
  }
}
</script>

<style lang="less">

</style>
