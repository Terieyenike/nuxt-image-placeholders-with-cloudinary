<template>
  <div class="lg:flex items-center justify-between">
    <div class="w-full px-8">
      <h1 class="md:text-3xl lg:text-5xl font-bold text-stone-800">IMAGE <span class="block">PLACEHOLDER</span></h1>
      <h2 class="mt-4 text-blue-700">using Cloudinary</h2>
    </div>

      <cld-image
        :public-id="publicId"
        loading="lazy"
        gravity="auto:subject"
        fetchFormat="auto"
        quality="auto"
        alt="An image example with Cloudinary"
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
      publicId: "his_view_kfqrfb",
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
