<script setup>
defineProps({
    post: {
        type: Object,
        required: true
    }
})
</script>

<template>
<div>
          <div class="header">
          <span>Written by {{ post.name }} on {{ post.date }}</span>
          <div>
            <button class="del material-icons">delete</button>
            <button class="save material-icons">bookmark_border</button>
          </div>
        </div>
        <h1>{{ post.title }}</h1>
        <p>{{ post.body }}</p>
</div>
</template>


<style lang="scss" scoped>
  
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.5rem;

    span {
      font-size: 0.95rem;
      color: #888;
    }

    div {
      display: flex;
      gap: 0.5rem;

      button {
        border: none;
        background: #f5f5f5;
        color: #444;
        padding: 0.5rem 1rem;
        border-radius: 6px;
        cursor: pointer;
        font-size: 1rem;
        transition: background 0.2s;

        &.del {
          background: #ffeaea;
          color: #d32f2f;

          &:hover {
            background: #ffcccc;
          }
        }

        &.save {
          background: #eafaf1;
          color: #388e3c;

          &:hover {
            background: #c8f7e2;
          }
        }

        &.material-icons {
          font-family: 'Material Icons', sans-serif;
        }
      }
    }
  }

  h2 {
    margin-top: 0;
    font-size: 2rem;
    color: #222;
  }

  p {
    font-size: 1.1rem;
    color: #555;
    margin-bottom: 0;
  }
</style>