<template>
  <div class="home">
    <nav-bar />
    <div v-if="isLogging" class="before-logging">
      <log-in />
    </div>
    <div class="logging-screen container" v-if="false">
      <div class="row">
        <div class="col-3"><FriendList /></div>
        <div class="col-7"><ChattingRoom /></div>
      </div>
    </div>
    <div class="fast-chat">
      <FastChatRoom />
    </div>
  </div>
</template>

<script>
import ChattingRoom from '@/components/ChattingRoom.vue';
import LogIn from '@/components/LogIn.vue';
import NavBar from '@/components/NavBar.vue';
import FriendList from '@/components/FriendList.vue';
import FastChatRoom from '@/components/FastChatRoom.vue';

export default {
  name: 'Home',
  components: {
    LogIn,
    NavBar,
    ChattingRoom,
    FriendList,
    FastChatRoom,
  },
  data() {
    return {
      isLogging: false,
    };
  },
};
</script>
