<template>
  <div>
    <section class="main-section-container flex flex-row md:flex-col">
      <!-- <section class="px-12 flex flex-row md:flex-col md:gap-8 md:items-center bg-gray-dark"> -->
      <div class="convert-text-container">
        <h1 class="convert-heading w-1/2">Convert and Optimize Your Images for the Web</h1>
        <p>
          Easily upload your images and convert them into smaller webp files for faster website
          loading.
        </p>
      </div>
      <div class="upload-image-box">
        <IconUploadImg
          class="w-full md:max-w-xs"
          :handleClick="handleUpload"
          style="max-width: 100%"
        />
      </div>
    </section>
    <section class="secondary-section-container">
      <h3 class="discover-heading">Discover the Power of Image Optimization</h3>
      <div class="discover-row flex flex-row md:flex-col">
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
            With our webapp, you can easily upload and convert your images into webp format,
            ensuring faster loading times for your website.
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
    </section>
  </div>
</template>
<script lang="ts">
import IconBox from '@/components/icons/IconBox.vue'
import IconUploadImg from '@/components/icons/IconUploadImg.vue'

export default {
  name: 'HomePage',
  components: {
    IconBox,
    IconUploadImg
  },
  methods: {
    handleUpload() {
      console.log('Uploaded clicked')
      alert('Upload clicked!')
    }
  }
}
</script>
<style>
.main-section-container {
  /* Header / 7 / */

  /* Auto layout */
  /* display: flex; */
  /* flex-direction: row; */
  /* flex-wrap: wrap; */
  justify-content: space-between;
  align-items: center;
  padding: 4rem 4rem;
  margin: 0px;

  /* min-height: 760px; */

  background: #3f3f3f;
  border-radius: 0px;
}

.convert-text-container {
  padding: 2rem;
  color: white;
}

.convert-heading {
  /* Medium length hero headline goes here */

  /* width: 560px; */
  /* height: 201px; */

  /* Heading/H1 */
  font-style: normal;
  font-weight: 700;
  font-size: 56px;
  line-height: 120%;
  padding: 0 0 2rem 0;
  /* or 67px */

  /* White */
  color: #ffffff;

  /* Inside auto layout */
  flex: none;
  order: 0;
  align-self: stretch;
  flex-grow: 0;
}

.upload-image-box {
  max-width: 100%; /* Ensure the image stays within its container */
  height: auto; /* Maintain aspect ratio */
  align-items: center;
  justify-content: center;
}

.secondary-section-container {
  /* Layout / 238 / */

  /* Auto layout */
  display: flex;
  flex-direction: column;

  align-items: center;
  padding: 10vh 10vw;
  gap: 80px;
  margin: 0px;

  /* White */
  background: #ffffff;
  border-radius: 0px;

  /* Inside auto layout */
  flex: 1;
  order: 1;
  align-self: stretch;
  flex-grow: 1;
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
  /* display: flex; */
  /* flex-direction: row; */
  justify-content: center;
  align-items: center;
  margin: 0px 60px 0px 60px;
  padding: 0px;
  gap: 48px;

  /* border-radius: 0px; */

  /* Inside auto layout */
  /* flex: none; */
  /* order: 1; */
  /* align-self: stretch; */
  /* flex-grow: 0; */
  flex: none;
  order: 1;
  flex-grow: 0;
}

.discover-column {
  /* Column */

  /* Auto layout */
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 0 0 2rem 0;
  margin: 0px;
  gap: 24px;

  width: auto;

  border-radius: 0px;
  text-align: center;

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
  flex-grow: 0;
}

/* @media only screen and (min-width: 768px) {
  .main-section-container {
    flex-direction: column;
  }
  .discover-row {
    flex-direction: column;
  }
} */
</style>
