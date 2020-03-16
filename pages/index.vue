<template>
  <div >
    <div>
      <!-- #Left Sidebar ==================== -->
      <LeftSidebar/>

      <!-- #Main ============================ -->
       <div class="page-container">
        <!-- ### $Topbar ### -->
          <HeaderNavbar/>

        <!-- ### $App Content ### -->
          <MainContent/>
       

        <!-- ### $App Footer ### -->
          <Footer/>

      </div>
    </div>
  </div>
  
</template>

<script>
import Rules from "../components/Rules";
import Sidebar from "../components/Sidebar";
import SidebarHeader from "../components/SidebarHeader";
import HeaderNavbar from "../components/HeaderNavbar";
import MainContent from "../components/MainContent";
import Footer from "../components/Footer"
import LeftSidebar from "../components/LeftSidebar";
export default { 
 components: {
    Rules,
    Sidebar,
    SidebarHeader,
    HeaderNavbar,
    MainContent,
    Footer,
    LeftSidebar
  },

 
}
</script>



<style lang="scss">
   $fa-font-path: "~font-awesome/fonts";
   @import '../node_modules/font-awesome/scss/font-awesome';
/* @import "./scss/custom-bootstrap"; */

</style>
