<template>
  <div class="card">
    <div class="card-body">
      <div class="card-title">朋友/聊天室列表</div>
      <div class="tab-name mb-3">
        <ul class="nav nav-tabs">
          <li class="nav-item">
            <a class="nav-link" aria-current="friends" href="#">朋友</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" aria-current="groups" href="#">群組</a>
          </li>
        </ul>
      </div>
      <div class="tab-item-list">
        <ul class="list-group">
          <li class="list-group-item">An item</li>
          <li class="list-group-item">A second item</li>
          <li class="list-group-item">A third item</li>
          <li class="list-group-item">A fourth item</li>
          <li class="list-group-item">And a fifth one</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FriendList',
};
</script>
