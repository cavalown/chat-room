<template>
  <div class="card log-in-on">
    <div class="card-body">
      <h3 class="card-title mb-3" v-if="isLogOn">註冊</h3>
      <h3 class="card-title mb-3" v-else>登入</h3>
      <div class="mb-3 input-group-sm">
        <input
          type="email"
          class="form-control"
          id="floatingInput"
          placeholder="name@example.com"
        />
      </div>
      <div class="mb-3 input-group-sm">
        <input
          type="string"
          class="form-control"
          id="floatingId"
          placeholder="暱稱 (非必要）"
        />
      </div>
      <div class="mb-3 input-group-sm">
        <input
          type="password"
          class="form-control"
          id="floatingPassword"
          placeholder="Password"
        />
      </div>
      <div class="buttons d-flex justify-content-end">
        <button
          type="button"
          class="btn btn-link btn-sm"
          v-if="isLogOn"
          @click="isLogOn = true"
        >
          尚未註冊？點此註冊!
        </button>
        <button type="button" class="btn btn-outline-success" v-if="isLogOn">
          註冊
        </button>
        <button type="button" class="btn btn-outline-success" v-else>
          登入
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'logIn',
  data() {
    return {
      isLogOn: false,
    };
  },
};
</script>

<style lang="scss">
.log-in-on {
  max-width: 300px;
  margin: 0 auto;
  h3 {
    font-family: 'Courier New', Courier, monospace;
    font-size: 20px;
    font-weight: bold;
  }
}
</style>
