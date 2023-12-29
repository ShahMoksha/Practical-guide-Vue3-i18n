<script setup></script>

<template>
  <div class="locale-switcher">
    <div class="locale-changer">
      <select v-model="$i18n.locale"  style="padding: 5px 15px;font-size: 16px;">
        <option
          v-for="locale in $i18n.availableLocales"
          :key="`locale-${locale}`"
          :value="locale"
        >
          {{ locale }}
        </option>
      </select>
    </div>
  </div>
</template>

<style scoped></style>
