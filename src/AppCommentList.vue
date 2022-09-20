<template>
  <div>
    <div class="card inline">
      <h3>Комментарии 1</h3>
      <button class="btn danger">Удалить</button>
    </div>
    <div class="card inline">
      <h3>Комментарии 2</h3>
      <button class="btn danger">Удалить</button>
    </div>
  </div>
  <div class="card center">
    <h4>Пусто</h4>
  </div>
</template>

<script>
export default {
  emits: ['load','remove'],
  name: "AppCommentList"
}
</script>

<style scoped>
  .inline {
     display: flex;
    justify-content: space-between;
    align-items: center;
  }
</style>
