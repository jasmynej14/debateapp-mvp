<template>
    <view class="feed-item">
        <text>{{ user.name }}</text>
        
    </view>
</template>

<script>
import Video from 'react-native-video';
export default {
    components:{
        Video
    },
    props:{
        user:{
            Type:Object
        }
    },
    data(){
        return{
            videoSource:{uri:'https://www.sample-videos.com/video/mp4/720/big_buck_bunny_720p_10mb.mp4'}
        }
    }
}
</script>

<style>
    .feed-item{
        background-color: cadetblue;
    }
</style>
