<template>
  <v-app>
    <v-main>
        <div>
          <b-navbar type="dark" variant="dark">
          <b-navbar-nav>
          <router-link to="/"><b-nav-item href="home">Home</b-nav-item></router-link>
          <router-link to="/profile"><b-nav-item href="profile">Profile</b-nav-item></router-link>
          <router-link to="/profiles"><b-nav-item href="profiles">Profiles</b-nav-item></router-link>
          <router-link to="/about"><b-nav-item href="about">About</b-nav-item></router-link>
          <b-nav-item-dropdown text="User" right>
          </b-nav-item-dropdown>
          </b-navbar-nav>
          </b-navbar>
          <router-view/>
        </div>
        <div>
              <b-button v-b-toggle.sidebar-1 id="sidebar_button">Toggle Sidebar</b-button>
              <b-sidebar id="sidebar-1" title="Sidebar" shadow>
                <div class="px-3 py-2">
                  <p>
                    Cras mattis consectetur purus sit amet fermentum. Cras justo odio, dapibus ac facilisis
                    in, egestas eget quam. Morbi leo risus, porta ac consectetur ac, vestibulum at eros.
                  </p>
                  <b-img src="https://picsum.photos/500/500/?image=54" fluid thumbnail></b-img>
                </div>
              </b-sidebar>
            </div>
    </v-main>
  </v-app>
</template>
<script>
//import HelloWorld from './components/HelloWorld';
export default {
  name: 'App',

  components: {
    //HelloWorld,
  },

  data: () => ({
    //
  }),
};
</script>
<style>
  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif; -webkit-font-smoothing: antialiased; -moz-osx-font-smoothing: grayscale; text-align: center; color: #2c3e50;
  }

  #nav {
    padding: 30px;
  }

  #nav a {
    font-weight: bold;
    color: #2c3e50;
  }

  #nav a.router-link-exact-active {
    color: #42b983;
  }

  #sidebar_button{
    position: fixed;
    left: 50%;
    bottom: 20px;
    transform: translate(-50%, -50%);
    margin: 0 auto;
  }
</style>
