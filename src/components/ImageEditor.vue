const icona = require("tui-image-editor/dist/svg/icon-a.svg");
<template>
  <div class="page">
    <div class="imageEditorApp">
      <tui-image-editor ref="editor" :include-ui="useDefaultUI" :options="options"></tui-image-editor>
    </div>
  </div>
</template>
<script>
import { ImageEditor } from "@toast-ui/vue-image-editor";

export default {
  name: "ImageEditor",
  components: {
    "tui-image-editor": ImageEditor
  },
  data() {
    return {
      useDefaultUI: true,
      options: {
        cssMaxWidth: window.innerWidth,
        cssHeight: 800,
        initMenu: "filter"
      }
    };
  },   
};
</script>
<style scoped>
.imageEditorApp {
  width: 95vw;
  height: 95vh;
}

.tui-image-editor-header-logo{
  display: none;
}
</style>