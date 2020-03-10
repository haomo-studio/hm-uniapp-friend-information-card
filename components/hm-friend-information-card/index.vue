<template>
  <div class="hm-friend-information-card">
    <div class="box">
      <image class="primary" :src="options.primary" />
      <div class="side">
        <div class="namClass">
          <text class="name">{{ options.name }}</text>
        </div>
        <image class="titleImg" :src="options.titleImg" />
        <text class="address">{{ options.address }}</text>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'HmFriendInformationCard',
  props: {
    dataId: {
      type: String,
      default: 'hm-friend-information-card'
    },
    options: {
      type: Object,
      default: function() {
        return {
          primary:
            '/static/hm-friend-information-card/images/img_24031_0_1.png',
          name: '张三',
          titleImg:
            '/static/hm-friend-information-card/images/img_24031_0_0.png',
          address: '深圳'
        };
      }
    }
  },
  data() {
    return {};
  },
  methods: {}
};
</script>
<style>
@import './index.response.css';
</style>
