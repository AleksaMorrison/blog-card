<script setup>
</script>

<template>
  <div class="card-wrap">
    <img src="/assets/images/illustration-article.svg" alt="blog illustration">
    <div class="card-content">
      <p class="category">Learning</p>
      <p class="date">Published 21 Dec 2023</p>
      <a href="#">HTML & CSS foundations</a>
      <p class="description">These languages are the backbone of every website, defining structure, content, and presentation.</p>
    </div> 
    <div class="author">
        <img src="/assets/images/image-avatar.webp" alt="Greg Hooper">
        <p>Greg Hooper</p>
      </div> 
  </div>
</template>
<style lang="scss" scoped>
.card-wrap {
  display: flex;
  flex-direction: column;
  justify-content: center;
  background-color: var(--white);
  border-radius: 20px;
  padding: var(--spacing400);
  gap: var(--spacing400);
  max-width: 327px;
  box-shadow: var(--shadow);
  height: min-content;
  border: 1px solid var(--gray950);
  box-shadow: 8px 8px 0px black;

  @media (min-width: 376px) {
    max-width: 384px;
  }

  & .card-content{
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    gap: var(--spacing150);

    p {
      margin: 0;
    }

    & .category {
      color: var(--gray950);
      background-color: var(--yellow);
      padding: 4px 12px;
      width: fit-content;
      font-weight: 700;
    }

    & .description {
      color: var(--gray500);
    }

    & a {
      font-size: 24px;
      font-weight: 700;
      color: var(--gray950);
      margin: 0;

      &:hover,
      &:focus{
        color: var(--yellow);
      }
    }
  }

  & img {
    width: 100%;
    border-radius: 10px;
  }

  & .author {
    display: flex;
    align-items: center;
    gap: var(--spacing200);

    & img {
      width: 32px;
      height: 32px;
      border-radius: 50%;
    }

    & p {
      color: var(--gray950);
      font-weight: 700;
      font-size: 14px;
      margin: 0;
    }
  }
}
</style>