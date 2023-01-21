<template>
  <div class="repos__item">
    <div class="repos__left" >
      <h2>{{ repos.name }}</h2>
      <p>Кол-во звёзд: {{ repos.stargazers_count }}⭐⭐⭐</p>
      <p>Дата добавления: {{ new Date(repos.created_at).toLocaleDateString()}}</p>
    </div>
    <div class="repos__right">
      <a :href="repos.html_url" class="repos__link">ПОСЕТИТЬ</a>
    </div>
  </div>
</template>

<script>

export default {
props:{
  repos:Object
}
};
</script>

<style>
</style>