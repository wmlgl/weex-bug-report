<template>
  <div class="container">
    <slider class="slider" :auto-pay="true">
      <scroller class="scroller">
        <text>AAA</text>
        <image :src="imgA" style="width:300px;height:300px;background-color:orange" />
      </scroller>
      <scroller class="scroller">
        <text>BBB</text>
        <image :src="imgB" style="height:2000px" />
      </scroller>
      <scroller class="scroller">
        <text>CCC</text>
        <image :src="imgA" style="height:2000px" />
      </scroller>
    </slider>
  </div>
</template>
<script>
export default {
  data() {
    return {
      imgA: "local:///a",
      imgB: "local:///b",
      // imgC: "local:///c"
      imgC:
        "https://img.alicdn.com/tfs/TB1M2MYqzTpK1RjSZKPXXa3UpXa-1152-912.png"
    };
  }
};
</script>
<style>
.container {
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
}
.slider {
  flex: 1;
}
.scroller {
  position: absolute;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  background-color: #eeeeee;
  overflow: scroll;
}
</style>