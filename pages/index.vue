<template>
  <section id="container">
    <h1>Anmitsu</h1>
    <div class="manifest">
      <h2>Step1. manifest.jsonの作成</h2>
      <p>manifest.jsonは、アドオンの情報やバージョンを記述する、アドオンの構成上必要なファイルです。</p>
      <p>
        <label><input type="radio" name="addonType" v-model="picked">リソースパック</label>
        <label><input type="radio" name="addonType" v-model="picked">ビヘイビアパック</label>
        <label><input type="radio" name="addonType" v-model="picked">ScriptingAPI</label>
      </p>
      <h4>アドオン名</h4>
      <input v-model="addonName" placeholder="アドオン名を入力">
      <h4>アドオンの説明</h4>
      <textarea v-model="addonDescription" placeholder="説明を入力"></textarea>
      <h4>アドオンのバージョン</h4>
      <p><input type="number" max="9" min="0" v-model="v0">.<input type="number" max="9" min="0" v-model="v1">.<input type="number" max="9" min="0" v-model="v2"></p>
      <button>生成</button>
      <h4>出力</h4>
      <p><textarea v-model="output"></textarea></p>
    </div>

  </section>
</template>

<script>
  // var app = new Vue({
  //   // el: '#container',
  //   // data:{
  //   //   output: ''
  //   // }
  // })
</script>

<style>

</style>
