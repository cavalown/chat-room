<template>
  <div class="card" style="max-width: 800px; margin: 0 auto">
    <div class="card-body">
      <div class="card-title border">快速聊天</div>
      <div class="message-block" v-for="message in messages" :key="message.id">
        <div class="user-info d-flex">
          <h2 class="userName fs-5 mr-3">{{ message.user }}</h2>
          <h4 class="timeStamp fs-6">{{ message.timeStamp }}</h4>
        </div>
        <h3 class="message">{{ message.text }}</h3>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FastChatRoom',
  data() {
    return {
      messages: [
        {
          user: 'QQ',
          text: '哈哈哈',
          timeStamp: '2022-04-01 16:03',
          id: 'nfnobnvigorjbipr',
        },
        {
          user: 'TT',
          text: '喔',
          timeStamp: '2022-04-01 16:04',
          id: 'bbohjptiengoew',
        },
      ],
    };
  },
};
</script>
