<style lang="less">
  @import "../src/components/styles/index.less";
</style>
<style scoped>
nav { margin-bottom: 40px; }
ul { display: flex; flex-wrap: wrap; }
li { display: inline-block; }
li + li { border-left: solid 1px #bbb; padding-left: 10px; margin-left: 10px; }
.container{ padding: 10px 40px 0; }
.v-link-active { color: #bbb; }
</style>
<template>
    <div class="container">
      <nav>
        <ul>
          <li><router-link to="/affix">Affix</router-link></li>
          <li><router-link to="/icon">Icon</router-link></li>
        </ul>
      </nav>
      <router-view></router-view>
    </div>
</template>
<script>
  module.exports = {
    data: function() {
      return {

      }
    },
    mounted: function() {

    },
    beforeDestroy: function() {

    },
    methods: {

    }
  }
</script>
