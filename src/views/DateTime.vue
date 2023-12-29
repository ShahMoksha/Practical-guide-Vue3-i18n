<script setup></script>

<template>
  <div class="about">
    <h2>{{ $t("dateTime") }}</h2>
    <br />
    <ul class="a">
      <li>
        <span class="text-details"> Date Formatting short:</span>
        {{ $d(new Date(), "shortFormat") }}
      </li>
      <li>
        <span class="text-details"> Date Formatting long:</span>
        {{ $d(new Date(), "longDate") }}
      </li>
      <li>
        <span class="text-details"> Date -- long Month:</span>
        {{ $d(new Date(), "longMonth") }}
      </li>
      <li>
        <span class="text-details"> Date and time Formatting long:</span>
        {{ $d(new Date(), "long") }}
      </li>
    </ul>
  </div>
</template>

<style scoped>
.about {
  padding: 50px 100px;
  font-size: 22px;
}
</style>
