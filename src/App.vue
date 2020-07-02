<template>
  <div id="app">
    <ImageEditor />
  </div>
</template>
<script>

import ImageEditor from "./components/ImageEditor";

export default {
  components: {
    ImageEditor
  }
}
</script>

<style lang="scss">
.page {
  padding: 20px;
}
button,
.btn.btn-primary {
  margin-right: 10px !important;
}
.button-toolbar {
  margin-bottom: 10px;
}
</style>