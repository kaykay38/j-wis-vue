<script setup lang="ts"></script>

<template>
  <div class="main-section-container">
    <div class="convert-text-container">
      <h1 class="font-roboto font-bold text-3xl">Convert and Optimize Your Images for the Web</h1>
      <p>
        Easily upload your images and convert them into smaller webp files for faster website
        loading.
      </p>
    </div>
    <div class="upload-image-box"></div>
  </div>
  <div class="secondary-section-container">
    <h3 class="discover-heading">Discover the Power of Image Optimization</h3>
    <div class="discover-row">
      <div class="discover-column">
        <IconBox />
        <h5 class="discover-subtitle">Effortlessly Optimize Your Website's Images</h5>
        <p>
          Our webapp accepts images and converts them into smaller webp images, perfect for
          optimizing your website's performance.
        </p>
      </div>
      <div class="discover-column">
        <IconBox />
        <h5 class="discover-subtitle">Transform Your Images with Ease</h5>
        <p>
          With our webapp, you can easily upload and convert your images into webp format, ensuring
          faster loading times for your website.
        </p>
      </div>
      <div class="discover-column">
        <IconBox />
        <h5 class="discover-subtitle">Boost Your Website's Performance</h5>
        <p>
          Experience the benefits of optimized images by using our webapp to convert your images
          into webp format.
        </p>
      </div>
    </div>
  </div>
</template>
<script lang="ts">
import { defineComponent } from 'vue'
import IconBox from '@/components/icons/IconBox.vue'

export default defineComponent({
  name: 'HomePage',
  components: {
    IconBox
  }
})
</script>
<style>
.main-section-container {
  /* Header / 7 / */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  padding: 0px 64px;

  height: 960px;

  background: #3f3f3f;
  border-radius: 0px;

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

.convert-text-container {
  padding: 20px;
  color: white;
}

.upload-image-box {
  /* Upload Box */

  margin: 0 auto;
  width: calc(50vw - 20px);

  /* Inside auto layout */
  flex: none;
  order: 1;
  flex-grow: 0;
}

.secondary-section-container {
  /* Layout / 238 / */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 112px 64px;
  gap: 80px;

  height: 588px;

  /* White */
  background: #ffffff;
  border-radius: 0px;

  /* Inside auto layout */
  flex: none;
  order: 2;
  flex-grow: 0;
}

.discover-heading {
  /* Heading/H3 */
  font-style: normal;
  font-weight: 700;
  font-size: 40px;
  line-height: 120%;
  /* identical to box height, or 48px */
  text-align: center;

  /* Black */
  color: #000000;

  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 0;
}

.discover-row {
  /* Row */

  /* Auto layout */
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start;
  margin: 0px 20px 0px 20px;
  padding: 0px;
  gap: 48px;

  height: 236px;

  border-radius: 0px;

  /* Inside auto layout */
  flex: none;
  order: 1;
  align-self: stretch;
  flex-grow: 0;
}

.discover-column {
  /* Column */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 0px;
  gap: 24px;

  height: 236px;
  width: calc((100vw - 150px) / 3);

  border-radius: 0px;

  /* Inside auto layout */
  flex: none;
  order: 0;
  flex-grow: 1;
}

.discover-subtitle {
  /* Heading */

  /* Heading/H5 */
  font-style: normal;
  font-weight: 700;
  /* font-size: 24px; */
  line-height: 140%;
  /* or 34px */
  text-align: center;

  /* Black */
  color: #000000;

  /* Inside auto layout */
  flex: none;
  order: 0;
  align-self: stretch;
  flex-grow: 0;
}
</style>
