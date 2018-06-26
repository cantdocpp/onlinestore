<template>
  <div id="app">
    <div id="nav" uk-sticky="sel-target: .uk-navbar-container; cls-active: uk-navbar-sticky">
      <nav class="uk-navbar-container" uk-navbar="dropbar: true" style="background: white" >
        <div class="uk-navbar-left">
            <ul class="uk-navbar-nav">
                <li class="uk-active logo-word"><a href="#" style="font-size: 20px; font-weight: 600"><img src="logo.ico" style="width: 70px; height: 70px; margin: auto">PBL</a></li>
                <li class="uk-parent"><a href=""></a></li>
                <li><a href=""></a></li>
            </ul>
        </div>
        <div class="uk-navbar-left">
          <ul class="uk-navbar-nav">
            <li>
              <a class="uk-navbar-toggle" href="#" style="color: black">
                <i class="material-icons">menu</i> <span style="color: black">Shop</span>
                <div class="uk-navbar-dropdown uk-navbar-dropdown-width-3">
                          <div class="uk-navbar-dropdown-grid uk-child-width-1-3" uk-grid>
                              <div>
                                  <ul class="uk-nav uk-navbar-dropdown-nav">
                                      <li class="uk-active"><a href="#">Active</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-header">Header</li>
                                      <li><a href="#">Item</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-divider"></li>
                                      <li><a href="#">Item</a></li>
                                  </ul>
                              </div>
                              <div>
                                  <ul class="uk-nav uk-navbar-dropdown-nav">
                                      <li class="uk-active"><a href="#">Active</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-header">Header</li>
                                      <li><a href="#">Item</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-divider"></li>
                                      <li><a href="#">Item</a></li>
                                  </ul>
                              </div>
                              <div>
                                  <ul class="uk-nav uk-navbar-dropdown-nav">
                                      <li class="uk-active"><a href="#">Active</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-header">Header</li>
                                      <li><a href="#">Item</a></li>
                                      <li><a href="#">Item</a></li>
                                      <li class="uk-nav-divider"></li>
                                      <li><a href="#">Item</a></li>
                                  </ul>
                              </div>
                          </div>
                      </div>
              </a>
            </li>
          </ul>

      </div>
      <div class="uk-navbar-right">
        <div class="uk-offcanvas-content">
          <span class="uk-margin-small-right uk-button uk-button-default uk-margin-small-right" uk-icon="icon: cart; ratio: 1.3" uk-toggle="target: #offcanvas-reveal" style="border: none"></span>
          <div id="offcanvas-reveal" uk-offcanvas="mode: reveal; flip: true; overlay: true">
            <div class="uk-offcanvas-bar">
                <button class="uk-offcanvas-close" type="button" uk-close></button>
                <h3>Title</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.</p>
            </div>
          </div>
        </div>
      </div>
    </nav>
      <!-- <router-link to="/">Home</router-link> -->
    </div>
    <router-view/>
  </div>
</template>

<script>

</script>

<style lang="scss">
  .logo-word {
    letter-spacing: 10px;
  }
</style>
