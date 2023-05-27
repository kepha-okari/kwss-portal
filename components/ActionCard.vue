<template>
<div class="row">
  <b-button class="card action-card" @click="handleSubmit">
    <img src="../assets/chatting.png" height="40px" width="40px" />
    <p>Send Bills</p>
  </b-button>
</div>

</template>

<script>
export default {
  methods: {
    handleSubmit() {
      alert('Salute!');
    }
  }
}
</script>

<style>
.action-card{
  margin: 25px;
}
</style>