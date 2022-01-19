<template>
  <div>
    <b-navbar toggleable="lg" type="light" variant="light">
      <b-container>
        <b-navbar-brand href="#">
          <img
            src="~/assets/logo_text-scaled-177x58.png"
            style="max-height: 45px; width: auto"
            alt="Kitten"
          />
        </b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto">
            <b-nav-item href="#">Home</b-nav-item>
            <b-nav-item-dropdown text="Products" right>
              <b-dropdown-item href="#">
                Point of Sale System (POS)
              </b-dropdown-item>
              <b-dropdown-item href="#">
                WooCommerce Point of Sale (WooPOS)
              </b-dropdown-item>
              <b-dropdown-item href="#"
                >Hotel Management System (HMS)
              </b-dropdown-item>
              <b-dropdown-item href="#"
                >Restaurant Management System</b-dropdown-item
              >
              <b-dropdown-item href="#">Desktop SMS System</b-dropdown-item>
              <b-dropdown-item href="#"
                >Admission Management System</b-dropdown-item
              >
              <b-dropdown-item href="#"
                >Property Management System</b-dropdown-item
              >
              <b-dropdown-item href="#"
                >Result Publishing System</b-dropdown-item
              >
              <b-dropdown-item href="#"
                >Laundry Management System</b-dropdown-item
              >
            </b-nav-item-dropdown>
            <b-nav-item href="#">Services</b-nav-item>
            <b-nav-item href="#">About</b-nav-item>
            <b-nav-item href="#">Blog</b-nav-item>
            <b-nav-item href="#">Contact</b-nav-item>
            <b-nav-item href="https://wovoui.netlify.app" target="_balnk">wovoui</b-nav-item>
          </b-navbar-nav>
        </b-collapse>
      </b-container>
    </b-navbar>
  </div>
</template>
