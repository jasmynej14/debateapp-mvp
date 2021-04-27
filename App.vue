<template>
  <view class="container">

    <text>Title</text>
    
    <Feed/>
    
  </view>
</template>

<script>
import Feed from "./components/Feed";
export default {
  components: { Feed },
  data() {
    return {
      message: "Hello World"
    };
  },
  methods: {
    exclaim() {
      this.message += "!";
    }
  },
};
</script>

<style>
.container {
  flex: 1;
  background-color: white;
  margin-top: 70px;
}
.text-color-primary {
  color: blue;
  font-size: 30;
}
</style>