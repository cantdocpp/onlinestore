<template>
  <div id="app">
    <div id="nav" uk-sticky="sel-target: .uk-navbar-container; cls-active: uk-navbar-sticky">
      <nav class="uk-navbar-container" uk-navbar="dropbar: true" style="background: white" >
        <div class="uk-navbar-left">
            <ul class="uk-navbar-nav">
                <router-link to="/">
                <li class="uk-active logo-word" style="text-decoration: none"><a href="#" style="font-size: 20px; font-weight: 600; color: black; text-decoration: none"><img src="logo.ico" style="width: 70px; height: 70px; margin: auto;">PBL</a></li>
                <li class="uk-parent"><a href=""></a></li>
                </router-link>
            </ul>
        </div>
        <div class="uk-navbar-left">
          <ul class="uk-navbar-nav">
            <li>
              <a class="uk-navbar-toggle" href="#" style="color: black">
                <i class="material-icons">menu</i> <span style="color: black;">Shop</span>
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
        <ul class="uk-iconnav">
          <li><router-link to="/login"><a href="" uk-icon="icon: user" style="color: black"></a></router-link></li>
      </ul>
        <div class="uk-offcanvas-content">
          <span class="uk-margin-small-right uk-button uk-button-default uk-margin-small-right" uk-icon="icon: cart; ratio: 1.3" uk-toggle="target: #offcanvas-reveal" style="border: none"></span>
          <div id="offcanvas-reveal" uk-offcanvas="mode: reveal; flip: true; overlay: true">
            <div class="uk-offcanvas-bar">
                <button class="uk-offcanvas-close" type="button" uk-close style="color: black"></button>
                <h3 class="offcanvas-font" style="color: black">your cart is empty</h3>
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

  .uk-offcanvas-bar {
    background: white;
  }

  h3 .offcanvas-font {
    color: black
  }

  li::hover {
    border-bottom: none
  }

  .uk-link::hover {
    color: white
  }

  a:hover  {
    text-decoration: none
  }
</style>
