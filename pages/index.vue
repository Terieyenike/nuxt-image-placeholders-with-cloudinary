<template>
  <div class="lg:flex items-center h-screen">
    <div class="w-full px-8">
      <h1 class="md:text-5xl lg:text-4xl font-bold text-stone-800">
        IMAGE LOADING <span class="block">PLACEHOLDER</span>
      </h1>
      <h2 class="md:mb-4 lg:mt-3 text-blue-700">using Cloudinary and Nuxt</h2>
    </div>

    <cld-image
      :public-id="publicId"
      loading="lazy"
      gravity="auto:subject"
      fetchFormat="auto"
      quality="auto"
      alt="Calm teri sitting"
    >
      <cld-placeholder type="pixelate" />
    </cld-image>
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data() {
    return {
      publicId: "image-placeholders/teri",
    };
  },
};
</script>

<style>
.cld-image {
  object-fit: cover;
  border-radius: 10px;
}
</style>
