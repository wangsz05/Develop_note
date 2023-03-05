# vue

# 1 vue 模板文件

模板文件demo

```vue
<!--  -->
<template>
  <div/>
</template>

<script>
// 这里可以导入其他文件（比如：组件，工具js，第三方插件js，json文件，图片文件等等）
// 例如：import 《组件名称》 from '《组件路径》'

export default {
  // import引入的组件需要注入到对象中才能使用
  components: {},
  data() {
    // 这里存放数据
    return {

    }
  },
  // 监听属性 类似于data概念
  computed: {},
  // 监控data中的数据变化
  watch: {},
  // 生命周期 - 创建完成（可以访问当前this实例）
  created() {

  },
  // 生命周期 - 挂载完成（可以访问DOM元素）
  mounted() {

  },
  beforeCreate() {}, // 生命周期 - 创建之前
  created() {}, // 生命周期 - 创建之后
  beforeMount() {}, // 生命周期 - 挂载之前
  mounted() {}, //生命周期 - 挂载之后
  beforeUpdate() {}, // 生命周期 - 更新之前
  updated() {}, // 生命周期 - 更新之后
  beforeDestroy() {}, // 生命周期 - 销毁之前
  destroyed() {}, // 生命周期 - 销毁完成
  activated() {}, // 如果页面有keep-alive缓存功能，这个函数会触发
  // 方法集合
  methods: {

  }
}

</script>
<style lang='less' scoped>
//@import url(); 引入公共css类

</style>

```

# 2 layout头和layout底部不变

可以参考:https://blog.csdn.net/abcwanglinyong/article/details/83538532

可以用`<div>`标签定义好头部和底部，在定义路由动态的标签在页面中，`<div>` `<router-view></router-view>`，然后通过路由的变换可以动态的切换页面的内容



