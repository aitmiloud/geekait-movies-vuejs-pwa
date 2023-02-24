<template>
  <nav :class="$style.nav">
    <img src="~/assets/images/geekait2.png" alt="logo2" srcset="" class="logo" style="width:26em; height:5em;">
  </nav>
</template>

<script>
export default {
  props: {

  },
};
</script>

<style lang="scss">
@import '~/assets/css/utilities/_variables.scss';

</style>

<style lang="scss" module>
@import '~/assets/css/utilities/_variables.scss';

@media all and (max-width: 520px) {
/* Logo for Mobile */
.logo {
  width:26em;
  height:5em;
}}

.nav {
  position: fixed;
  top: 0;
  right: 0;
  left: 0;
  z-index: 5;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 6rem;
  padding: 0 5.5rem;
  background-color:rgba(0, 0, 0, 0.7);

}

.text {
  margin: 0;
  overflow: hidden;
  font-size: 3rem;
  text-overflow: ellipsis;
  white-space: nowrap;
}

</style>
