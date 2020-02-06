<template>
  <div class="home">
    <h1>Vue Notes</h1>
    <div class="todo-list">
      <div class="todo-list__item">
        <div class="todo-list__header"><i class="icon-sticky-note"></i>Buy something</div>
        <div class="todo-list__group">
          <div class="todo-list__subitem">Milk</div>
          <div class="todo-list__subitem">Bread</div>
          <div class="todo-list__subitem">Potates</div>
        </div>
      </div>
      <div class="todo-list__item">
        <div class="todo-list__header"><i class="icon-sticky-note"></i>Buy something</div>
        <div class="todo-list__group">
          <div class="todo-list__subitem">Milk</div>
          <div class="todo-list__subitem">Bread</div>
          <div class="todo-list__subitem">Potates</div>
        </div>
      </div>
      <div class="todo-list__item">
        <div class="todo-list__header"><i class="icon-sticky-note"></i>Buy something</div>
        <div class="todo-list__group">
          <div class="todo-list__subitem">Milk</div>
          <div class="todo-list__subitem">Bread</div>
          <div class="todo-list__subitem">Potates</div>
        </div>
      </div>
      <div class="todo-list__item">
        <div class="todo-list__header"><i class="icon-sticky-note"></i>Buy something</div>
        <div class="todo-list__group">
          <div class="todo-list__subitem">Milk</div>
          <div class="todo-list__subitem">Bread</div>
          <div class="todo-list__subitem">Potates</div>
        </div>
      </div>

      <div class="todo-list__footer">
        <a class="add-note" href="#" title="add note">
          <span>Add Note</span>
        </a>
      </div>
    </div>

    <button class="button button--create">
      <i class="icon-plus"></i>
    </button>
  </div>
</template>

<script>
export default {
  name: 'home',
};
</script>

<style lang="scss">
.todo-list {
  flex: none;
  max-width: 960px;
  width: 100%;
  margin-bottom: 20px;
  border-radius: 10px;

  &__item {
    margin-bottom: 20px;
  }

  &__header {
    margin-bottom: 10px;
    font-weight: bold;
    font-size: 18px;
  }

  &__group {
    margin-bottom: 10px;
  }

  &__subitem {
    position: relative;
    padding-left: 10px;
    color: #251954;

    &::before {
      position: absolute;
      top: 50%;
      margin-top: -1px;
      left: 0;
      width: 5px;
      height: 1px;
      background-color: #ccc;
      content: '';
    }
  }
}

.button.button--create {
  position: fixed;
  display: flex;
  justify-content: center;
  align-items: center;
  bottom: 50px;
  right: 50px;
  width: 70px;
  height: 70px;
  border-radius: 50%;
  background-color: #6e47f1;
  color: #fff;
  font-size: 34px;
  cursor: pointer;
  transition: 0.4s;

  .icon-plus {
    position: relative;
    top: -1px;
  }

  &:hover {
    opacity: 0.9;
  }
}
</style>
