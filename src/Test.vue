<template>
    <div class="box1">
        <h3>这是Test.vue---{{ username }}</h3>
        <button @click="changeName">变化</button>
    </div>
    
</template>

<script>
    // 默认导出，这是固定写法
    export default {
        // 在vue中data 数据必须是一个函数
        data() {
            return {
                username: 'mm'
            }
        },
        // 方法
        methods: {
            changeName() {
                this.username = '哇哈哈'
            }
        },
        // 当前组件的侦听器
        watch: {},
        // 当前组件的计算属性
        computed: {},
        // 当前组件中的过滤器
        filters: {}
    }
</script>

<style lang="less">
   .box1 {
       background-color: pink;
       h3 {
       color: red;
   }
   };
  
</style>