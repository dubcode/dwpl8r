<template>
  <div class="breadcrumbs --row">
    <ul>
      <li class="active">
        <span>1</span>
      </li>
      <li class="current">
        <span>2</span>
      </li>
      <li>
        <span>3</span>
      </li>
      <li>
        <span>4</span>
      </li>
      <li>
        <span>5</span>
      </li>
    </ul>
  </div>
</template>

<style lang="scss" scoped>
.breadcrumbs {
  margin: 0 0 1em 0;
  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    text-align: center;
    li {
      display: inline-block;
      height: 40px;
      width: 40px;
      span {
        align-items: center;
        border: 2px solid #00e1bd;
        border-radius: 100%;
        color: #00e1bd;
        display: flex;
        font-weight: 600;
        height: 40px;
        justify-content: center;
        text-align: center;
        width: 40px;
      }
    }
    li.current span {
      background: #413793;
      border: 2px solid #413793;
      color: #fff;
    }
    li.active span {
      background: #00e1bd;
      border: 2px solid #00e1bd;
      color: #fff;
    }
  }
}
</style>
