<template>
  <div>
    <h2>分类</h2>
    <div class="wrapper">
      <ul class="content">
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
        <li>111</li>
      </ul>
    </div>
  </div>

</template>

<script>
import BScroll from 'better-scroll'
export default {
  name: 'Category',
  created () {
    // this.scroll = new BScroll('.wrapper', {

    // })
  },
  data () {
    return {
      scroll: null,
    }
  },
  mounted () {
    this.scroll = new BScroll('.wrapper', {
        probeType:3,
    });

    this.scroll.on('scroll',(position)=>{
        console.log(position)
    })
  }
}
</script>

<style scoped>
.wrapper {
  height: 150px;
  background-color: red;
  overflow: hidden;
}
</style>