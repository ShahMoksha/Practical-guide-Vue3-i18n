<script setup></script>

<template>
  <div class="about">
    <h2>{{ $t("pluralization") }}</h2>
    <ul>
      <li>[pass value: 0] {{ $t("pl.car", 0) }}</li>
      <li>[pass value:1 ] {{ $t("pl.car", 1) }}</li>

      <br>
      <li>[pass value:0] {{ $t("pl.apple", 0) }}</li>
      <li>[pass value: 1] {{ $t("pl.apple", 1) }}</li>
      <li>[pass value: 10] {{ $t("pl.apple", 10, { count: 10 }) }}</li>
    </ul>
  </div>
</template>

<style scoped>
.about {
  padding: 50px 100px;
  font-size: 22px;
}
</style>
