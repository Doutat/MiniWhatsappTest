<template>
  <f7-page>
    <!-- Statusbar -->

    <f7-navbar title="Test App">
      <f7-nav-right>
        <f7-link searchbar-enable icon-f7="search"></f7-link>
        <f7-link popover-open=".popover-menu" icon-f7="more_vertical"></f7-link>
      </f7-nav-right>
      <f7-searchbar expandable></f7-searchbar>
    </f7-navbar>

    <f7-popover class="popover-menu">
      <f7-list>
        <f7-list-item popover-close title="Dialog"></f7-list-item>
        <f7-list-item popover-close title="Tabs"></f7-list-item>
        <f7-list-item popover-close title="Side Panels"></f7-list-item>
        <f7-list-item popover-close title="List View"></f7-list-item>
        <f7-list-item popover-close title="Form Inputs"></f7-list-item>
      </f7-list>
    </f7-popover>

     


<!-- Views/Tabs container -->
 
    <!-- Tabbar for switching views-tabs -->
    <f7-toolbar tabbar labels top>
      <f7-link tab-link="#view-disc" tab-link-active  text="DISC."></f7-link>
      <f7-link tab-link="#view-statut" text="STATUT"></f7-link>
      <f7-link tab-link="#view-appels" text="APPELS"></f7-link>
    </f7-toolbar>

    <!-- Your main view/tab, should have "view-main" class. It also has "tab-active" class -->
    <f7-views>
    <f7-view id="view-disc" main tab tab-active url="/"></f7-view>

    <!-- Catalog View -->
    <f7-view id="view-statut" name="statut" tab url="/statut/"></f7-view>

    <!-- Settings View -->
    <f7-view id="view-appels" name="appels" tab url="/appels/"></f7-view>
    </f7-views>
  </f7-page>
</template>
