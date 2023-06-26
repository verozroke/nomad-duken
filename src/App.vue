<script setup>
import HeaderVue from '@/components/HeaderVue.vue'
import FooterVue from '@/components/FooterVue.vue'
</script>

<template>
  <div style="overflow: hidden">
    <header-vue />
    <div class="wrapper">
      <main>
        <router-view v-slot="{ Component }">
          <transition name="routering" mode="out-in">
            <component :is="Component"></component>
          </transition>
        </router-view>
      </main>
      <footer-vue />
    </div>
  </div>
</template>

<style lang="scss">
main {
  flex: 1 1 auto;
}

.wrapper {
  display: flex;
  flex-direction: column;
  overflow: hidden;
  min-height: 100vh;
  background-color: #fff;
}

.routering {
  &-enter-from {
    opacity: 0;
    transform: translateX(1000px);
  }
  &-enter-active {
    transition: all 0.3s ease-out;
  }
  &-leave-to {
    opacity: 0;
    transform: translateX(-1000px);
  }
  &-leave-active {
    transition: all 0.3s ease-in;
  }
}

::-webkit-scrollbar {
  width: 13px;

  background-color: transparent;
  &-track {
    background-color: transparent;
    margin-block: 0.5em;
  }
  &-thumb {
    background-color: rgba(47, 47, 47, 0.836);
    border-radius: 100vw;
    transition: 0.4s;
    border: 4px solid rgba(0, 0, 0, 0);
    background-clip: padding-box;
    &:hover {
      background-color: rgb(28, 28, 28);
      transition: 0.4s;
    }
  }
}
</style>
