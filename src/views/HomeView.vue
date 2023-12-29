<script setup>
import { useI18n } from "vue-i18n";
const { t } = useI18n();
</script>

<template>
  <main>
    <div class="about">
      <h1 style="text-align: center; font-weight: bold;">{{ $t("home.header") }}</h1>
      <ul class="a">
        <li>
          <span class="text-details">Translation with $t() (method):</span>
          {{ $t("home.$tfunction") }}
        </li>
        <li>
          <span class="text-details">Translation with import useI18n function:</span
          >
          {{ t("home.iUseI18n") }}
        </li>
        <li>
          <span class="text-details">when text is not found in locale:</span>
          {{ $t("home.fallbackText") }}
        </li>
        <li>
          <span class="text-details">Named interpolation:</span>
          {{ $t("home.popularItem", { item: "123456" }) }}
        </li>
        <li>
          <span class="text-details">List interpolation:</span>
          {{ $t("home.list", ["hey","Good noon"]) }}
        </li>
        <li>
          <span class="text-details">Literal interpolation(email):</span>
          {{ $t("home.address", { account: "foo", domain: "domain.com" }) }}
        </li>
       
      </ul>
           
    </div>
  </main>
</template>

<style scoped>
.about {
  padding: 50px 100px;
  font-size: 22px;
}
.flex {
  display: flex;
  align-items: center;
  padding-bottom: 7px;
}
.text-details {
  /* text-decoration: underline; */
  padding-right: 15px;
  color: #05386B;
    font-weight: bold;
}
ul.a {
  list-style: square;
}
</style>
