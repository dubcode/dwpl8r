<template>
  <div class="pop --row" style="margin: 0 0 1em 0;">
    <div class="--ctr">
      <popper
        trigger="clickToOpen"
        :options="{
          placement: 'top',
          modifiers: { offset:
            { offset: '0,10px' }
          }
        }"
      >
        <div class="popper">
          Tooltip content goes here
        </div>
        <button slot="reference" class="popper__button">
          ?
        </button>
      </popper>
    </div>
  </div>
</template>

<script>
import Popper from 'vue-popperjs'
import 'vue-popperjs/dist/vue-popper.css'
export default {
  components: {
    'popper': Popper
  }
}
</script>

<style lang="scss" scoped>
.pop {
  overflow: visible;
}
.popper__button {
  background: #413793;
  border-radius: 100%;
  border: none;
  color: #fff;
  height: 20px;
  margin: 0;
  outline: 0;
  padding: 0;
  width: 20px;
}
</style>
