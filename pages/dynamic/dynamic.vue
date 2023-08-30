<template>
  <view class="cu-card case" :class="isCard ? 'no-card' : ''">
    <view class="cu-item shadow">
      <view class="image">
        <image class="w100"
          src="https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500"
          mode="widthFix">
        </image>
        <view class="cu-tag bg-blue">新人</view>
        <view class="cu-bar bg-shadeBottom"> <text
            class="text-cut">我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。</text></view>
      </view>
      <view class="cu-list menu-avatar">
        <view class="cu-item">
          <view class="cu-avatar round lg"
            style="background-image:url(https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500);">
          </view>
          <view class="content flex-sub">
            <view class="text-grey">凯尔</view>
            <view class="text-gray text-sm flex justify-between">
              刚刚
              <view class="text-gray text-sm">
                <!-- <text class="cuIcon-attentionfill margin-lr-xs"></text> -->
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="eye" size="28" margin-left="10" margin-right="10"
                  label="10"></u-icon>
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="thumb-up" size="28" margin-left="10"
                  margin-right="10" label="20"></u-icon>
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="heart-fill" size="28" margin-left="10"
                  margin-right="10" label="30"></u-icon>
              </view>
            </view>
          </view>
        </view>
      </view>
    </view>
    <view class="cu-item shadow">
      <view class="image">
        <image class="w100"
          src="https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500"
          mode="widthFix">
        </image>
        <view class="cu-tag bg-blue">新人</view>
        <view class="cu-bar bg-shadeBottom"> <text
            class="text-cut">我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。我已天理为凭，踏入这片荒芜，不再受凡人的枷锁遏制。</text></view>
      </view>
      <view class="cu-list menu-avatar">
        <view class="cu-item">
          <view class="cu-avatar round lg"
            style="background-image:url(https://img2.baidu.com/it/u=640593135,209279600&fm=253&fmt=auto&app=138&f=JPEG?w=889&h=500);">
          </view>
          <view class="content flex-sub">
            <view class="text-grey">凯尔</view>
            <view class="text-gray text-sm flex justify-between">
              刚刚
              <view class="text-gray text-sm">
                <!-- <text class="cuIcon-attentionfill margin-lr-xs"></text> -->
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="eye" size="28" margin-left="10" margin-right="10"
                  label="10"></u-icon>
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="thumb-up" size="28" margin-left="10"
                  margin-right="10" label="20"></u-icon>
                <u-icon class="margin-lr-xs" label-color="#aaaaaa" name="heart-fill" size="28" margin-left="10"
                  margin-right="10" label="30"></u-icon>
              </view>
            </view>
          </view>
        </view>
      </view>
    </view>
  </view>
</template>

<script>
export default {
  data() {
    return {

    };
  },
  methods: {

  }
};
</script>

<style lang="scss" scoped>
.cu-card {
  display: block;
  overflow: hidden;

  &>.cu-item {
    display: block;
    background-color: #ffffff;
    overflow: hidden;
    border-radius: 5px;
    margin: 15px;
  }
}

.cu-card.case .image .cu-tag {
  position: absolute;
  right: 0;
  top: 0;
}

.bg-blue {
  background-color: #0081ff;
  color: #ffffff;
}

.cu-tag {
  font-size: 12px;
  vertical-align: middle;
  position: relative;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  box-sizing: border-box;
  padding: 0px 8px;
  height: 24px;
  font-family: Helvetica Neue, Helvetica, sans-serif;
  white-space: nowrap;
}

.cu-card.case .image .cu-bar {
  position: absolute;
  bottom: 0;
  width: 100%;
  background-color: transparent;
  padding: 0px 15px;
}

.bg-shadeBottom {
  background-image: linear-gradient(rgba(0, 0, 0, 0.01), rgba(0, 0, 0, 1));
  color: #ffffff;
}

.cu-bar {
  display: flex;
  position: relative;
  align-items: center;
  min-height: 52px;
  justify-content: space-between;
}

.text-cut {
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.cu-list.menu-avatar {
  overflow: hidden;
}

.cu-list.menu-avatar>.cu-item {
  position: relative;
  display: flex;
  padding-right: 5px;
  height: 72px;
  background-color: #ffffff;
  justify-content: flex-end;
  align-items: center;
}

.cu-list>.cu-item {
  transition: all .6s ease-in-out 0s;
  -webkit-transform: translateX(0px);
  transform: translateX(0px);
}

.cu-list.menu-avatar>.cu-item>.cu-avatar {
  position: absolute;
  left: 15px;
}

.cu-avatar.lg {
  width: 49px;
  height: 49px;
  font-size: 2em;
}

.cu-avatar {
  font-variant: small-caps;
  margin: 0;
  padding: 0;
  display: inline-flex;
  text-align: center;
  justify-content: center;
  align-items: center;
  background-color: #ccc;
  color: #ffffff;
  white-space: nowrap;
  position: relative;
  width: 33px;
  height: 33px;
  background-size: cover;
  background-position: center;
  vertical-align: middle;
  font-size: 1.5em;
}

.round {
  border-radius: 2600px;
}

.cu-list.menu-avatar>.cu-item .content.flex-sub {
  width: calc(100% - 49px - 31px - 10px);
}

.cu-list.menu-avatar>.cu-item .content {
  position: absolute;
  left: 75px;
  width: calc(100% - 49px - 31px - 62px - 10px);
  line-height: 1.6em;
}

.cu-list.menu-avatar>.cu-item .content>view:first-child {
  font-size: 15px;
  display: flex;
  align-items: center;
}

.text-grey,
.line-grey,
.lines-grey {
  color: #8799a3;
}

.flex-sub {
  flex: 1;
}

.text-gray,
.line-gray,
.lines-gray {
  color: #aaaaaa;
}

.text-sm {
  font-size: 12px;
}

.justify-between {
  justify-content: space-between;
}

.margin-lr-xs {
  margin-left: 5px;
  margin-right: 5px;
}

.flex {
  display: flex;
}

.cu-card.case .image {
  position: relative;

  .w100 {
    width: 100%;
    height: 100%;
  }
}
</style>
