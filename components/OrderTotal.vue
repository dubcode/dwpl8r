<template>
  <div class="--row">
    <div class="--ctr">
      <div class="order-description --row">
        <div>
          <p><b>Description</b></p>
        </div>
        <div>
          {{ order_description }}
        </div>
      </div>
      <div class="order-total --row">
        <div>
          <p><b>Order Total</b></p>
        </div>
        <div>
          <ul>
            <li>£ {{ order_total }}</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data () {
    return {
      order_description: '2 X Lorem ipsum dolor emit',
      order_total: '200.00'
    }
  }
}
</script>

<style lang="scss" scoped>
  .order-description {
    border-bottom: 1px solid #ccc;
    display: grid;
    grid-template-columns: 0.6fr 1.4fr;
    grid-template-rows: 1fr;
    margin: 0 0 1em 0;
    padding: 0 0 1em 0;
    li {
      color: #666;
      font-size: 0.9em;
      line-height: 1.4em;
    }
    p b {
      color: #000;
      font-weight: 600;
      font-size: 0.9em;
    }
  }
 .order-total {
    display: grid;
    grid-template-columns: 0.6fr 1.4fr;
    grid-template-rows: 1fr;
    margin: 0 0 1em 0;
    li {
      color: #666;
      font-size: 0.9em;
      line-height: 1.4em;
    }
    p b {
      color: #000;
      font-weight: 600;
      font-size: 0.9em;
    }
  }
</style>
