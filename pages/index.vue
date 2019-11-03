<template>
  <div class="--row">
    <div class="app">
      <logo />
      <strapline />
      <breadcrumbs />
      <order />
      <popper />
      <btn />
    </div>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Strapline from '~/components/Strapline.vue'
import Breadcrumbs from '~/components/Breadcrumbs.vue'
import Order from '~/components/Order.vue'
import Popper from '~/components/Popper.vue'
import Btn from '~/components/Btn.vue'
export default {
  components: {
    Logo,
    Strapline,
    Breadcrumbs,
    Order,
    Popper,
    Btn
  }
}
</script>
