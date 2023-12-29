<script setup></script>

<!-- <template>
  <div class="about">
   
  </div>
</template> -->

<style>
/* @media (min-width: 1024px) { */
/* .about { */
/* min-height: 100vh; */
/* display: flex; */
/* align-items: center; */
/* } */
/* } */
</style>

<template>
  <div class="about">
    <h1>{{ $t("about-title") }}</h1>
    <div>=================================</div>
    <h3>
     <span  class="text-details">Available Locales in application:</span> 
      {{ $i18n.availableLocales }}
    </h3>
    <h3>
    <span class="text-details"> selected locale is:</span> 
      {{ $i18n.locale }}
    </h3>
    <div>=================================</div>
    <br />
    <ul>
      <li>{{ $t("about-sh") }}</li>
      <br />
      <li>{{ $t("about-para1") }}</li>
      <li>{{ $t("about-para2") }}</li>
      <li>{{ $t("about-para3") }}</li>
    </ul>
  </div>
</template>

<style scoped>
.about {
  padding: 50px 100px;
  font-size: 22px;
}
.text-details {
  text-decoration: underline;
  padding-right: 15px;
}
</style>
