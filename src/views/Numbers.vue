<script setup></script>

<template>
  <div class="about">
    <h2>{{$t("numbers")}}</h2>
    <br />
    <ul class="a">
        <span>=======================</span>
        <li>
          <span class="text-details">Number Formatting:</span>
          {{ $n(7854, "currency") }}
        </li>
        <li>
          <span class="text-details">currency with Name:</span>
          {{ $n(7854, "currency", { currencyDisplay: "name" }) }}
        </li>
        <li>
          <span class="text-details"> 12.11612345 decimal fraction 2:</span>
          {{ $n(12.11612345, "decimal", { maximumFractionDigits: 2 }) }}
        </li>
        <li>
          <span class="text-details"> 12.11612345 decimal fraction 4:</span>
          {{ $n(12.11612345, "decimal", { maximumFractionDigits: 4 }) }}
        </li>
        <li>
          <span class="text-details"> 0.99123 percent Formatting: </span>
          {{ $n(0.99123, "percent") }}
        </li>
        <li>
          <span class="text-details"> 0.99123 percent fraction 2: </span>
          {{ $n(0.99123, "percent", { minimumFractionDigits: 2 }) }}
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
