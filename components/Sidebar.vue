<template>
  <div role="tablist">

    <ul class="sidebar-menu scrollable pos-r">
            <li class="nav-item mT-30 actived">
              <a class="sidebar-link" href="index.html">
                <span class="icon-holder">
                  <i class="c-blue-500 ti-home"></i>
                </span>
                <span class="title">Dashboard</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link'  @click="DisplayProfiles()">
                <span class="icon-holder">
                  <i class="c-brown-500 ti-email"></i>
                </span>
                <span class="title">Profiles</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link' href="compose.html">
                <span class="icon-holder">
                  <i class="c-blue-500 ti-share"></i>
                </span>
                <span class="title">Compose</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link' href="calendar.html">
                <span class="icon-holder">
                  <i class="c-deep-orange-500 ti-calendar"></i>
                </span>
                <span class="title">Calendar</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link' href="chat.html">
                <span class="icon-holder">
                  <i class="c-deep-purple-500 ti-comment-alt"></i>
                </span>
                <span class="title">Chat</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link' href="charts.html">
                <span class="icon-holder">
                  <i class="c-indigo-500 ti-bar-chart"></i>
                </span>
                <span class="title">Charts</span>
              </a>
            </li>
            <li class="nav-item">
              <a class='sidebar-link' href="forms.html">
                <span class="icon-holder">
                  <i class="c-light-blue-500 ti-pencil"></i>
                </span>
                <span class="title">Forms</span>
              </a>
            </li>
            <li class="nav-item dropdown">
              <a class="sidebar-link" href="ui.html">
                <span class="icon-holder">
                    <i class="c-pink-500 ti-palette"></i>
                  </span>
                <span class="title">UI Elements</span>
              </a>
            </li>
            <li class="nav-item dropdown">
                   
							<a role="tab"  href="#" v-b-toggle.accordion-1 variant="info" class="dropdown-toggle">
                    <span class="icon-holder">
                        <i class="c-orange-500 ti-layout-list-thumb"></i>
                    </span>
                    <span class="title">Tables</span>
                    <span class="arrow">
                      <i class="ti-angle-right"></i>
                    </span>
							</a>
				
							<b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
									<b-card-body class="padding-0">
										<ul class="dropdown-menu">
												<li>
												<a class='sidebar-link' href="basic-table.html">Basic Table</a>
												</li>
												<li>
												<a class='sidebar-link' href="datatable.html">Data Table</a>
												</li>
										</ul>
									</b-card-body>
							</b-collapse>

            </li>
            <!-- <li class="nav-item dropdown">
              <a class="dropdown-toggle" href="javascript:void(0);">
                <span class="icon-holder">
                    <i class="c-purple-500 ti-map"></i>
                  </span>
                <span class="title">Maps</span>
                <span class="arrow">
                    <i class="ti-angle-right"></i>
                  </span>
              </a>
              <ul class="dropdown-menu">
                <li>
                  <a href="google-maps.html">Google Map</a>
                </li>
                <li>
                  <a href="vector-maps.html">Vector Map</a>
                </li>
              </ul>
            </li> -->
            <!-- <li class="nav-item dropdown">
              <a class="dropdown-toggle" href="javascript:void(0);">
                <span class="icon-holder">
                    <i class="c-red-500 ti-files"></i>
                  </span>
                <span class="title">Pages</span>
                <span class="arrow">
                    <i class="ti-angle-right"></i>
                  </span>
              </a>
              <ul class="dropdown-menu">
                <li>
                  <a class='sidebar-link' href="blank.html">Blank</a>
                </li>                 
                <li>
                  <a class='sidebar-link' href="404.html">404</a>
                </li>
                <li>
                  <a class='sidebar-link' href="500.html">500</a>
                </li>
                <li>
                  <a class='sidebar-link' href="signin.html">Sign In</a>
                </li>
                <li>
                  <a class='sidebar-link' href="signup.html">Sign Up</a>
                </li>
              </ul>
            </li> -->
            <li class="nav-item dropdown" >
              <a class="dropdown-toggle" role="tab"  href="#" v-b-toggle.accordion-2 variant="info">
                <span class="icon-holder">
                  <i class="c-teal-500 ti-view-list-alt"></i>
                </span>
                <span class="title">Multiple Levels</span>
                <span class="arrow">
                  <i class="ti-angle-right"></i>
                </span>
              </a>
             		<b-collapse id="accordion-2" visible accordion="my-accordion" role="tabpanel">
									<b-card-body class="padding-0">
                      <ul class="dropdown-menu">
                        <li class="nav-item dropdown">
                          <a >
                            <span>Menu Item</span>
                          </a>
                        </li>
                        <li class="nav-item dropdown">
                          <a >
                            <span>Menu Item</span>
                            <span class="arrow">
                              <i class="ti-angle-right"></i>
                            </span>
                          </a>
                          <ul class="dropdown-menu">
                            <li>
                              <a href="javascript:void(0);">Menu Item</a>
                            </li>
                            <li>
                              <a href="javascript:void(0);">Menu Item</a>
                            </li>
                          </ul>
                        </li>
                      </ul>
              	</b-card-body >
              </b-collapse >
							
            </li>
          </ul>
  
  
  </div>

</template>

<style lang="scss" scoped>
	.padding-0{
		padding: 0
	}
	.dropdown-menu{
		display: block;
	}
</style>

<script>
    import Vue from 'vue'
    import VueRouter from 'vue-router'

    import { BootstrapVue } from 'bootstrap-vue'
    Vue.use(BootstrapVue)
    Vue.use(VueRouter)
    export default {
     name: "Sidebar",

     methods:{
       DisplayProfiles(){
         this.$router.push({name: 'Profiles'}) 
       }
     }
    }
    
</script>