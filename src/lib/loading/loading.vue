<template>
  <div :class="['u-main',{nofixed:!fixed}]"
    :style="`z-index:${zIndex};background:${bgColor};border-radius:${radius} ;`">
    <div class="u-content">
      <span :class="['loader-'+type,bottom?'u-bottom':'u-center']"></span>
    </div>
  </div>
</template>

<script>
  export default {
    name: "uLoading",
    data() {
      return {

      }
    },
    props: {
      zIndex: {
        type: Number,
        default: 1000
      },
      type: {
        type: Number,
        default: 1
      },
      fixed: {
        type: Boolean,
        default: true
      },
      bgColor: {
        type: String,
        default: "#263238"
      },
      radius: {
        type: String,
        default: "0px"
      },
      bottom: {
        type: Boolean,
        default: false
      }
    },
    created() {
      if(this.type < 1){
        this.type = 1
      }
      if(this.type > 92){
        this.type = 92
      }
    },
  }

</script>

<style scoped>
  @import url('../../assets/css/style.css');
  @import url('../../assets/css/animation.css');

</style>
