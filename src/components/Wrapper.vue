<template>
    <div class="wrapper">
        <slot></slot>
    </div>
</template>


<style lang="scss" scoped>
.wrapper {
  max-width: 700px;
  margin: 2rem auto;
  padding: 2rem;
  background: #fff;
  border-radius: 12px;
  box-shadow: 0 2px 16px rgba(0, 0, 0, 0.08);
}
</style>
