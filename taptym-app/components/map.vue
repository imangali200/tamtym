<template>
  <div>
    <div class="embed-map-fixed">
      <div class="embed-map-container">
        <iframe
          class="embed-map-frame"
          frameborder="0"
          scrolling="no"
          marginheight="0"
          marginwidth="0"
          src="https://maps.google.com/maps?width=600&height=400&hl=en&q=University%20of%20Oxford&t=&z=17&ie=UTF8&iwloc=B&output=embed"
        ></iframe
        ><a
          href="https://sprunkiretake.net"
          style="
            font-size: 2px !important;
            color: gray !important;
            position: absolute;
            bottom: 0;
            left: 0;
            z-index: 1;
            max-height: 1px;
            overflow: hidden;
          "
          >sprunki retake</a
        >
      </div>
    </div>
  </div>
</template>
<style>
.embed-map-fixed {
  position: relative;
  text-align: right;
  width: 600px;
  height: 400px;
}
.embed-map-container {
  overflow: hidden;
  background: none !important;
  width: 600px;
  height: 400px;
}
.embed-map-frame {
  width: 600px !important;
  height: 400px !important;
}
</style>
