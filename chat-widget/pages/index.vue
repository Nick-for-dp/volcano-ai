<script setup lang="ts">
const sessionName = 'default-session'
</script>

<template>
  <div class="chat-page">
    <ChatWidget :session-name="sessionName" />
  </div>
</template>

<style scoped>
.chat-page {
  width: 100%;
  min-height: 100vh;
  margin: 0;
  padding: 40px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f6f3ef;
}

.chat-page :deep(.chat-widget) {
  width: min(640px, 100%);
  height: min(78vh, 760px);
  max-height: calc(100vh - 80px);
  border: 1px solid rgba(0, 0, 0, 0.06);
  border-radius: 20px;
  box-shadow: 0 18px 48px rgba(0, 0, 0, 0.1);
  overflow: hidden;
}
</style>
