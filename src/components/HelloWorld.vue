<template>
  <h1>
    vue3仿美团项目
    <div>基础</div>
    <svg class="icon" aria-hidden="true">
        <use xlink:href="#icon-search"></use>
    </svg>
    <van-button type="primary">主要按钮</van-button>
  </h1>
  <Grandson/>
</template>

<script>
import {onMounted, reactive, toRef, toRefs, inject} from 'vue';
import Grandson from './Grandson.vue'
export default {
  name: 'HelloWorld',
  components: {
    Grandson
  },
  // setup函数在所有生命周期函数之后执行
  setup() {
    console.log('儿子xd', inject('xd'))
    onMounted(() => {

    })

    return {

    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang='less' scoped>
h1 {
  font-size: 20px;
  div {
    color: red;
  }
}
</style>
