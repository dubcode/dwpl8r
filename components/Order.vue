<template>
  <!-- wrapper start -->
  <div class="--row">
    <!-- ctr start -->
    <div class="--ctr">

      <!-- order description -->
      <div class="order-description --row">
        <div>
          <p><b>Description</b></p>
        </div>
        <div>
          {{ orderDescription }}
        </div>
      </div>

      <!-- order total -->
      <div class="order-total --row">
        <div>
          <p><b>Order Total</b></p>
        </div>
        <div>
          <ul>
            <li>£ {{ orderTotal }}</li>
          </ul>
        </div>
      </div>

      <!-- order deposit selection -->
      <form>
        <select class="form-select">
          <option value="40">
            £{{ depositOne }} / 10% Deposit
          </option>
          <option value="60">
            £{{ depositTwo }} / 20% Deposit
          </option>
          <option value="80">
            £{{ depositThree }} / 30% Deposit
          </option>
          <option value="100">
            £{{ depositFour }} / 40% Deposit
          </option>
        </select>
      </form>

      <!-- order payment terms selection -->
      <div class="box-list --row">
        <ul>
            <li>
            £{{ termOne }}* / month
            <span>for 3 months</span>
            </li>
            <li>
            £{{ termTwo }}* / month
            <span>for 6 months</span>
            </li>
            <li>
            £{{ termThree }}* / month
            <span>for 9 months</span>
            </li>
        </ul>
      </div>

    </div>
    <!-- ctr end -->
  </div>
  <!-- wrapper end -->
</template>

<script>
// initial order value & description
export default {
  data () {
    return {
      orderId: 1,
      orderDescription: '2 X Lorem ipsum dolor emit',
      orderTotal: '470.17',
      depositOne: '',
      depositTwo: '',
      depositThree: '',
      depositFour: '',
      termOne: '',
      termTwo: '',
      termThree: ''
    }
  },
  beforeMount () {
    this.createOptions()
  },
  methods: {
    createOptions () {
      // calculate deposit options
      this.depositOne = this.orderTotal / 10
      this.depositTwo = this.orderTotal / 5
      this.depositThree = this.orderTotal / 3.3333
      this.depositFour = this.orderTotal / 2.5
      this.depositOne = this.depositOne.toFixed(2)
      this.depositTwo = this.depositTwo.toFixed(2)
      this.depositThree = this.depositThree.toFixed(2)
      this.depositFour = this.depositFour.toFixed(2)
      // calculate term options
      this.termOne = this.orderTotal / 3
      this.termTwo = this.orderTotal / 6
      this.termThree = this.orderTotal / 9
      this.termOne = this.termOne.toFixed(2)
      this.termTwo = this.termTwo.toFixed(2)
      this.termThree = this.termThree.toFixed(2)
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
  .form-select {
    background: #fff url('data:image/svg+xml;charset=US-ASCII,%3Csvg%20xmlns%3D%22http%3A%2F%2Fwww.w3.org%2F2000%2Fsvg%22%20width%3D%22292.4%22%20height%3D%22292.4%22%3E%3Cpath%20fill%3D%22%23007CB2%22%20d%3D%22M287%2069.4a17.6%2017.6%200%200%200-13-5.4H18.4c-5%200-9.3%201.8-12.9%205.4A17.6%2017.6%200%200%200%200%2082.2c0%205%201.8%209.3%205.4%2012.9l128%20127.9c3.6%203.6%207.8%205.4%2012.8%205.4s9.2-1.8%2012.8-5.4L287%2095c3.5-3.5%205.4-7.8%205.4-12.8%200-5-1.9-9.2-5.5-12.8z%22%2F%3E%3C%2Fsvg%3E') no-repeat center right 20px;
    background-size: .65em auto, 100%;
    border: 1px solid #2abcc6;
    border-radius: .2em;
    color: #2abcc6;
    display: block;
    font-size: 1em;
    font-weight: 600;
    line-height: 1em;
    margin: 0 0 1em 0;
    padding: 1em;
    width: 100%;
    -moz-appearance: none;
    -webkit-appearance: none;
    appearance: none;
    :hover {
      border-color: #2abcc6;
    }
    :focus {
      border-color: #2abcc6;
      color: #2abcc6;
      outline: none;
    }
    option {
      font-weight:normal;
    }
  }
  .box-list ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
  }
  .box-list li {
    border: 1px solid #2abcc6;
    border-radius: .2em;
    color: #2abcc6;
    display: block;
    font-size: 1em;
    font-weight: 600;
    line-height: 1em;
    margin: 0 0 1em 0;
    padding: 1em;
    text-align: center;
    width: 100%;
    span {
      color: #666;
      display: block;
      font-weight: 400;
      padding: 0.5em 0 0 0;
    }
  }
</style>
