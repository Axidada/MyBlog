<template>
  <div class="common-footer">
    <p class="copyright">
      <a href="http://www.miibeian.gov.cn/" target="_blank">{{ siteInfo.icp }}</a>
      <span>|</span>
      {{ siteInfo.copyright }}
      <span>|</span>
      <span v-html="siteInfo.copyright_desc"></span>
    </p>
  </div>
</template>

<script type="text/ecmascript-6">
export default {
  data () {
    return {
      siteInfo: {
        icp: '鲁ICP备20021488号',
        copyright: '版权所有 © 2019 - 2019',
        copyright_desc: '以社交更多的IT志同道合的朋友一起分享自己的经验和知识,均已公开公正一起进步为目的'
      }
    }
  }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
  @import "../../common/stylus/theme.styl"
  .common-footer
    font-weight 300
    line-height 25px
    text-align center
    margin 15px 0
    color $default-title-color
    border-top 1px solid $default-border-color
    background $default-background-color
    @media only screen and (max-width: $responsive-sm)
      font-size 13px
    @media screen and (min-width: $responsive-sm)
      font-size 14px
    @media screen and (min-width: $responsive-md)
      font-size 15px
    @media screen and (min-width: $responsive-lg)
      font-size 15px
    .copyright
      margin 10px
      color $default-title-color
      a
        color $default-link-color
        &:hover
          color $default-link-hover-color
</style>
