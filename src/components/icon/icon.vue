<template>
  <i :class="classes" :style="styles"></i>
</template>

<script>
// very-vue 的图标使用开源项目 ionicons：http://ionicons.com/
const prefixCls = 'vvu-icon';

export default {
  name: 'Icon',
  props: {
    type: String,
    size: [Number, String],
    color: String
  },
  computed: {
    classes () {
      return `${prefixCls} ${prefixCls}-${this.type}`;
    },
    styles () {
      let style = {};

      if (this.size) {
        style['font-size'] = `${this.size}px`;
      }

      if (this.color) {
        style.color = this.color;
      }

      return style;
    }
  }
}
</script>

