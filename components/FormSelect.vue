<template>
  <div class="--row">
    <div class="--ctr">
      <form>
        <select class="form-select">
          <option value="40">
            £40.00 Deposit
          </option>
          <option value="60">
            £60.00 Deposit
          </option>
          <option value="80">
            £80.00 Deposit
          </option>
          <option value="100">
            £100.00 Deposit
          </option>
        </select>
      </form>
    </div>
  </div>
</template>

<style lang="scss" scoped>
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
</style>
