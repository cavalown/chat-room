<template>
  <div class="card">
    <div class="card-body">
      <div class="card-title">
        {{ chatRoomName }}
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'ChattingRoom',
  data() {
    return {
      chatRoomName: 'Micky',
    };
  },
};
</script>
