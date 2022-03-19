<template>
  <div class="login">
    <img alt="Vue logo" src="./assets/logo.png" />
    <br />
    <input type="password" v-model="passwordLama" placeholder="Password Lama" />
    <input type="password" v-model="passwordBaru" placeholder="Password Baru" />
    <button>Ganti Password</button>
  </div>
</template>
<script>
export default {
  name: "LupaPassword",
};
</script>
