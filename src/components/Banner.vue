<template>
  <div class="banner">
    <ul class="flex-row small-links">
      <li>More:</li>
      <li class="blue-text">All posts</li>
      <li class="blue-text">Artists</li>
      <li class="blue-text">News</li>
      <li class="blue-text">Downloads</li>
      <li class="blue-text">Tutorials</li>
      <li class="blue-text">Videos</li>
      <li class="blue-text">Loop</li>
      <li class="blue-text">One Thing</li>
    </ul>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.banner {
  min-width: 100%;
  background-color: #eee;
  display: flex;
  justify-content: center;
  padding: 4.16667vw 1rem;
  margin: 4.08333vw 0;
  text-align: center;

  ul {
    display: flex;
    align-items: center;
    flex-wrap: wrap;
  }

  li {
    margin-left: 18px;
    font-size: 1.5rem;
    line-height: 1.5;
    font-weight: 700;
  }
}
</style>
