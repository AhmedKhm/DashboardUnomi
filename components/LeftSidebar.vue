<template>
    <div>
      <!-- #Left Sidebar ==================== -->
        <div class="sidebar">
            <div class="sidebar-inner">
                
                    <!-- ### $Sidebar Header ### -->
                    <SidebarHeader/>
                    
                    <!-- ### $Sidebar Menu ### -->
                    <Sidebar/>
            
                </div>
            </div>
    </div>
</template>


<script>
import SidebarHeader from "../components/SidebarHeader";
import Sidebar from "../components/Sidebar";

    export default {
        name:"LeftSidebar",
        components:{
            SidebarHeader,
            Sidebar
        }

    }
</script>

<style lang="scss" scoped>

</style>