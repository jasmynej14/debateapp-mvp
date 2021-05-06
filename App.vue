<template>
  <nb-container class="home">
    <header/>
    <nb-content padder>
      <main-feed/>
    </nb-content>
    <nav-bar/>
  </nb-container>
</template>

<script>
import Vue from "vue-native-core";
import NavBar from './components/NavBar';
import Header from './components/Header';
import MainFeed from './components/MainFeed';
import Profile from './components/Profile';
import Notifications from './components/Notifications';
import { VueNativeBase } from "native-base"
import { Ionicons } from "@expo/vector-icons";


Vue.use(VueNativeBase);
Vue.component("ionicons", Ionicons);
export default {
  components : {NavBar,Header,MainFeed,Profile,Notifications},
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