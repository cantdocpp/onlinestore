<template>
  <div id="carousel">
    <!-- <i class="material-icons">menu</i> -->
    <div class="uk-position-relative uk-visible-toggle uk-light" uk-slideshow="ratio: 7:3; animation: push">
        <ul class="uk-slideshow-items">
            <li>
                <img src="https://getuikit.com/docs/images/light.jpg" alt="" uk-cover>
            </li>
            <li>
                <img src="https://getuikit.com/docs/images/dark.jpg" alt="" uk-cover>
            </li>
            <li>
                <img src="https://getuikit.com/docs/images/light.jpg" alt="" uk-cover>
            </li>
        </ul>
        <a class="uk-position-center-left uk-position-small uk-hidden-hover" href="#" uk-slidenav-previous uk-slideshow-item="previous"></a>
        <a class="uk-position-center-right uk-position-small uk-hidden-hover" href="#" uk-slidenav-next uk-slideshow-item="next"></a>

    </div>
  </div>
</template>
<script>
export default {
  name: "",
  data: () => ({

  })
}
</script>
<style lang="scss" scoped>
#carousel {
  margin-top: 30px
}
</style>
