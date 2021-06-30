<template>
  <div class="header flex-row">
    <div class="flex-row">
      <Logo />
      <ul class="flex-row medium-hidden">
        <li>Live</li>
        <li>Push</li>
        <li>Link</li>
        <li>Shop</li>
        <li>Packs</li>
        <li>Help</li>
        <li>More 
          <span>
            <img class="plus-icon" src="../assets/icons/plus.svg">
          </span>
        </li>
      </ul>
    </div>

    <ul class="flex-row">
      <li class="blue-text">Try Live for free</li>
      <li class="small-links">Log in or register</li>
    </ul>
  </div>
</template>

<script>
import Logo from "./Logo.vue";

export default {
  name: "Header",
  components: {
    Logo,
  },
};
</script>

<style scoped lang="scss">
.header {
  display: flex;
  justify-content: space-between;
  padding: 1.25rem 0;
  margin: 0 2.5rem;
  height: auto;
  width: auto;
  font-size: 20px;
  font-weight: 500;
}

ul {
  align-items: center;
}

li {
  margin: 0 1.3rem;
  font-size: 1.25rem;
  font-weight: 700;
  cursor: pointer;
  
}

.plus-icon{
  display: inline;
  width: 13px;
  height: 13px;
  margin-left: 3px;
}
</style>
