<script lang="ts">
import { defineComponent } from "vue";
// Uncomment import and local "components" registration if library is not registered globally.
// import { LeewardUiSample } from '@/entry.esm';

export default defineComponent({
  name: "ServeDev",
  // components: {
  //  LeewardUiSample,
  // }
  data() {
    return {
      counter: 1,
    };
  },
});
</script>

<template>
  <div id="app">
    <le-app block>
      <le-flex>
        <le-button class="grow" @click="counter++">
          <le-icon>wi-plus</le-icon>Add
        </le-button>
      </le-flex>
      <le-flex justify-center>{{counter}}</le-flex>
      <le-form>
        <le-input name="test-input">Label</le-input>
      </le-form>
    </le-app>
  </div>
</template>
