<template>
  <div class="container">
    <app-alert :alert="alert" @close="alert = null" ></app-alert>
      <form class="card" >
        <h2>Работа с базой комментариев</h2>
        <div class="form-control">
          <label for="comment">Введите комментарии</label>
          <input type="text" id="comment">
        </div>
        <button class="btn primary">Добавить коментарии</button>
      </form>
    <app-loader v-if="loading"></app-loader>
    <app-comment-list></app-comment-list>
  </div>
</template>

<script>
import AppCommentList from "@/AppCommentList";
import AppAlert from "@/AppAlert";
import AppLoader from "@/AppLoader"

export default {
  data() {
    return {
      name: '',
      comment: [],
      alert: null,
      loading: false
    }
  },
  components: {AppCommentList, AppAlert, AppLoader}
}
</script>

<style>

</style>
