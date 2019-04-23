<template>
<f7-app :params="f7params">
 <!-- Statusbar -->
    <f7-statusbar></f7-statusbar>    

<!-- Navbar -->
<!--<f7-navbar title="Test App" >
  <f7-nav-right>
    <f7-link class="searchbar-enable" data-searchbar=".searchbar-demo" icon-ios="f7:search" icon-aurora="f7:search" icon-md="material:search"></f7-link>
    <f7-link popover-open=".popover-menu" icon-f7="more_vertical"></f7-link>
  </f7-nav-right>
  <f7-searchbar
      class="searchbar-demo"
      expandable
      search-container=".search-list"
      search-in=".item-title"
      :disable-button="!$theme.aurora"
    >  
    </f7-searchbar>   
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

 -->



<f7-page :page-content="true">
  <f7-navbar title="Test App" >
  <f7-nav-right>
    <f7-link class="searchbar-enable" data-searchbar=".searchbar-demo" icon-ios="f7:search" icon-aurora="f7:search" icon-md="material:search"></f7-link>
    <f7-link popover-open=".popover-menu" icon-f7="more_vertical"></f7-link>
  </f7-nav-right>
  <f7-searchbar
      class="searchbar-demo"
      expandable
      search-container=".search-list"
      search-in=".item-title"
      :disable-button="!$theme.aurora"
    >  
    </f7-searchbar>   
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
 <f7-views tabs class="safe-areas">
    <!-- Your main view/tab, should have "view-main" class. It also has "tab-active" class -->
    <f7-view id="view-disc" main tab tab-active url="/"></f7-view>

    <!-- status View -->
    <f7-view id="view-statut" name="statut" tab url="/statut/"></f7-view>

    <!-- appels View -->
    <f7-view id="view-appels" name="appels" tab url="/appels/"></f7-view>

  </f7-views>
</f7-page>








  
  

  

</f7-app>
</template>
<script>
  import cordovaApp from '../js/cordova-app.js';
  import routes from '../js/routes.js';

  export default {
    data() {
      return {
        // Framework7 Parameters
        f7params: {
          id: 'io.framework7.myapp', // App bundle ID
          name: 'MyProjectMessagerie', // App name
          theme: 'auto', // Automatic theme detection
         

          // App routes
          routes: routes,



          // Input settings
          input: {
            scrollIntoViewOnFocus: !!this.$device.cordova,
            scrollIntoViewCentered: !!this.$device.cordova,
          },
          // Cordova Statusbar settings
          statusbar: {
            overlay: this.$device.cordova && this.$device.ios || 'auto',
            iosOverlaysWebView: true,
            androidOverlaysWebView: false,
          },
        },

        // Login screen data
        username: '',
        password: '',
      }
    },
    methods: {
      alertLoginData() {
        this.$f7.dialog.alert('Username: ' + this.username + '<br>Password: ' + this.password);
      }
    },
    mounted() {
      this.$f7ready((f7) => {
        // Init cordova APIs (see cordova-app.js)
        if (f7.device.cordova) {
          cordovaApp.init(f7);
        }
        // Call F7 APIs here
      });
    }
  }
</script>

<style>
.safe-areas
{
/*margin-top: -140px;*/
}
</style>
