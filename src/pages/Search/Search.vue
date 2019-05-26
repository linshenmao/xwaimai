<template>
  <section class="search">
      <form class="search_form" action="#">
        <input type="search" name="search" placeholder="请输入商家或美食名称" class="search_input">
        <input type="submit" name="submit" class="search_submit" value="搜索">
      </form>
    </section>
</template>

<script>
export default {
}
</script>

<style lang="stylus" scoped>
@import '../../common/stylus/mixins.styl'
.search
  width 100%
  .search_form
    clearFix()
    background-color #fff
    padding 12px 8px
    input
      height 35px
      padding 0 4px
      border-radius 2px
      font-weight bold
      outline none
      &.search_input
        float left
        width 80%
        border 4px solid #f2f2f2
        font-size 14px
        color #333
        background-color #f2f2f2
      &.search_submit
        float right
        width 18%
        border 4px solid #FF6347
        font-size 16px
        color #fff
        background-color #FF6347
        border-radius 5px
</style>
