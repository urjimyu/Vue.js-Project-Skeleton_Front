<template>
  <div class="item">
    <div class="icon">○</div>
    <div>
      <p>{{ data.category }}</p>
      <p>{{ data.amount.toLocaleString() }}원</p>
    </div>
  </div>
</template>

<script setup>
defineProps({ data: Object });
</script>

<style scoped>
.item {
  display: flex;
  align-items: center;
  border-bottom: 1px solid #ddd;
  padding: 8px 0;
}
.icon {
  width: 32px;
  height: 32px;
  background: #ccc;
  border-radius: 50%;
  margin-right: 12px;
}
</style>
