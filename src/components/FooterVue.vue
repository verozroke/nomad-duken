<template>
  <div class="footer">
    <div>{{ new Date().getFullYear() }} — <strong>Nomad Duken</strong></div>
  </div>
</template>

<script setup></script>

<style scoped lang="scss">
.footer {
  height: 50px;
  display: flex;
  align-items: center;
  padding: 0 20px;
  color: #fff;
  background-color: #000;
  font-family: 'DM Serif Display', serif;
}
</style>
