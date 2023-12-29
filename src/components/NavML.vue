<script setup>
import LocaleSwitcher from "./LocaleSwitcher.vue";

import { useI18n } from "vue-i18n";
const { t } = useI18n();
</script>

<template>
  <div class="nav">
    <div class="nav__start">
      <RouterLink to="/">{{ t("Home") }} </RouterLink>
      <RouterLink to="/about">{{ t("About") }} </RouterLink>
      <RouterLink to="/pluralization">{{ t("pluralization") }} </RouterLink>
      <RouterLink to="/dateTime">{{ t("dateTime") }} </RouterLink>
      <RouterLink to="/numbers"> {{t("numbers")}}</RouterLink>
    </div>

    <div class="nav__end">
      <p class="user-greeting">{{ $t("user_greeting", { name: "Sam" }) }}</p>
      <LocaleSwitcher />
    </div>
  </div>
</template>

<style scoped>
.nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-align: left;
  padding: 1rem;
  color: #fff;
  background-color: #05386B;
  font-size: 18px;
}

.nav__start,
.nav__end {
  display: flex;
  align-items: center;
}

.nav img {
  margin-right: 1rem;
}

.nav a {
  margin-right: 1.5rem;
  font-weight: bold;
  color: #fff;
  text-decoration: none;
}
.user-greeting {
  margin-right: 1rem;
}
</style>
<style>
[dir="rtl"] .user-greeting {
  margin-right: 0;
  margin-left: 1rem;
}
</style>
