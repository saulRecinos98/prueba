<template>
    <div class="header-main is-sticky" :class="isTransparent">
        <div class="container">
            <div class="header-wrap">
                <!-- logo -->
                <Logo></Logo>
                <!-- mobile action -->
                <MobileAction></MobileAction>
                <!-- heder search -->
                <HeaderSearch></HeaderSearch>
                <!-- Menu -->
                <Menu classname="btn-dark"></Menu>
                <div class="header-overlay"></div>
            </div><!-- .header-warp-->
        </div><!-- .container-->
    </div><!-- .header-main-->
</template>
<script>
// @ is an alias to /src
import Logo from '@/components/common/Logo.vue'
import MobileAction from '@/components/common/MobileAction.vue'
import HeaderSearch from '@/components/common/HeaderSearch.vue'
import Menu from '@/components/common/Menu.vue'

export default {
  name: 'HeaderMain',
  props: ['isTransparent'],
  components: {
    Logo,
    MobileAction,
    HeaderSearch,
    Menu
  }
}
</script>
