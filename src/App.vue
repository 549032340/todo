<template>
  <div class="main">
    <section class="header">
      <input type="text" />
    </section>
    <section>
      <ul class="todo">
        <li class="todo-item">
          <label>
            <input type="checkbox" /><span>奔驰</span>
            <button class="todo-button">删除</button>
          </label>
        </li>
        <li class="todo-item">
          <label>
            <input type="checkbox" /><span>宝马</span>
            <button class="todo-button">删除</button>
          </label>
        </li>
        <li class="todo-item">
          <label>
            <input type="checkbox" /><span>奥迪</span>
            <button class="todo-button">删除</button>
          </label>
        </li>
      </ul>
    </section>
    <section class="footer">
      <label>
        <input type="checkbox" />
        已完成1/全部3
      </label>
      <button class="todo-button ">清除已完成任务</button>
    </section>
  </div>
</template>

<style lang="less">
.main {
  width: 50%;
  margin: auto;
  text-align: center;
  border: 1px solid #ccc;
  padding: 15px;
  margin-top: 30px;
  border-radius: 5px;
}
.header {
  input {
    width: 100%;
    font-size: 20px;
    padding: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
    box-sizing: border-box;
    &:focus {
      outline: 0;
      border: 1px solid transparent;
      box-shadow: 0px 0px 8px 0px #1a71cc;
    }
  }
}
.todo {
  margin-top: 15px;
  text-align: left;
  border: 1px solid #ccc;
  border-radius: 5px;
}
.todo-item {
  padding: 5px;
  height: 30px;
  line-height: 30px;
  border-bottom: 1px solid #ccc;
  &:last-child {
    border-bottom: 0;
  }
  span {
    padding-left: 5px;
  }
  button {
    float: right;
    margin-top: 3px;
  }
}
.footer {
  margin: 20px 0 5px 0;
  text-align: left;
  button {
    float: right;
  }
}
</style>
