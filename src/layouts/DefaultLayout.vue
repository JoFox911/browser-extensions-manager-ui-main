<template>
  <div class="default-layout">
    <div class="page-content">
      <AppHeader />
      <main class="main-content">
        <router-view />
      </main>
    </div>
  </div>
</template>

<script setup>
import AppHeader from '@/components/AppHeader.vue'
</script>

<style scoped>
.default-layout {
  min-height: 100vh;
  min-width: 100vw;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.page-content {
  padding: var(--spacing-lg) var(--spacing-md);
  max-width: 1200px;
  width: 100%;
}

.main-content {
  flex: 1;
}
</style>
