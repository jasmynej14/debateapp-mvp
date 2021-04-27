<template>
   <scroll-view class="feed">
        <text>Feed</text>
        <feed-item v-for="user in users" :key="user.name" :user="user" class="feed-item"/>
   </scroll-view> 
</template>

<script>
import FeedItem from './FeedItem'

export default {
    components: { FeedItem },
    data(){
        return{
           users: [
               {name:"Jasmyne",content:"Video"},
               {name:"Jasmyne1",content:"Video"},
               {name:"Jasmyne2",content:"Video"},
               {name:"Jasmyne3",content:"Video"},
               {name:"Jasmyne4",content:"Video"}
           ] 
        }
    }
}
</script>

<style>

    .feed{
        background-color: beige;
        padding: 50px;
    }

    .feed-item{
        margin-bottom: 20px;
    }
</style>