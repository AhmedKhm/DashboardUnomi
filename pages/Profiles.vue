<template>
    <div >
    <div>
    
      <LeftSidebar/>
       <div class="page-container">
       
          
          <HeaderNavbar/> 
        
          <ProfileMainContent/>
          
          <Footer/>

      </div>
    </div>
  </div>
</template>

<script>
    import ProfileMainContent from "../components/ProfilesComponents/ProfileMainContent"
    import Sidebar from "../components/Sidebar";
    import SidebarHeader from "../components/SidebarHeader";
    import HeaderNavbar from "../components/HeaderNavbar";
    import Footer from "../components/Footer"
    import LeftSidebar from "../components/LeftSidebar";
    export default {
    components: {
        ProfileMainContent,
        Sidebar,
        SidebarHeader,
        HeaderNavbar,
        Footer,
        LeftSidebar
  },
        
    }
</script>

<style lang="scss" scoped>

</style>