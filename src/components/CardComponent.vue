<script>
export default {
  name: "CardComponent",
};
</script>

<template>
  <div class="col-33-img">
    <div class="content">
      <img class="object" src="../../img/1.webp" alt="" />
      <img class="object-hidden" src="../../img/1b.webp" alt="" />
      <button class="heart bg-white top-position right-position">
        &hearts;
      </button>
    </div>
    <span class="positioned-boxes bg-red boldness">-50%</span>
    <span class="positioned-boxes bg-green left-position boldness"
      >Sostenibilità</span
    >
    <div>Levi's</div>
    <div class="item-name boldness">RELAXED FIT TEE UNISEX</div>
    <span class="red-text boldness">14,99&euro;</span>
    <span class="text-line">29,99&euro;</span>
  </div>
</template>
