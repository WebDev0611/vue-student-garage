<template>
<!-- Navbar -->
    <nav class="navbar navbar-expand-lg student-garage-nav navbar-dark" data-navbar="sticky">
      <div class="container">

        <div class="navbar-left">
          <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
          <a class="navbar-brand" href="index.html">
            <img class="logo-dark" src="/static/assets/img/NavBar-Logo-Dark.png" alt="logo">
          </a>
        </div>
        <section class="navbar-mobile">
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
          <span class="navbar-divider d-mobile-none"></span>

          <ul class="nav nav-navbar mx-auto">
            <li class="nav-item">
              <a class="nav-link" href="#">Profiles <span class="arrow"></span></a>
              <nav class="nav">
                <a class="nav-link" href="demo/bootstrap.html">Students</a>
                <a class="nav-link" href="demo/dropbox.html">Investors</a>
                <a class="nav-link"> <router-link :to="{ name: 'ProfilePage' }">Your Profile</router-link></a>
              </nav>
            </li>

            <li class="nav-item">
              <a class="nav-link"> <router-link :to="{ name: 'QAMain' }">Q & A</router-link></a>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#">Resources <span class="arrow"></span></a>
              <nav class="nav">
                <a class="nav-link"> <router-link :to="{ name: 'EventsMain' }">Events</router-link></a>
                <a class="nav-link"> <router-link :to="{ name: 'EducationMain' }">Education</router-link></a>
                <a class="nav-link"> <router-link :to="{ name: 'JobsMain' }">Jobs</router-link></a>
              </nav>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#">Demo Day <span class="arrow"></span></a>
              <nav class="nav">
                <a class="nav-link"> <router-link :to="{ name: 'DiscoverMain' }">Discover</router-link></a>
                  <a class="nav-link"> <router-link :to="{ name: 'PostProductMain' }">Post Product</router-link></a>
              </nav>
            </li>

            <li class="nav-item">
              <a class="nav-link" href="#">Your Account <span class="arrow"></span></a>
              <nav class="nav">
                <a class="nav-link"> <router-link :to="{ name: 'ProfilePage' }">Your Profile</router-link></a>
                <a class="nav-link"> <router-link :to="{ name: 'MessagesMain' }">Messages</router-link></a>
                <a class="nav-link"> <router-link :to="{ name: 'MyProducts' }">Your Products</router-link></a>
                <a class="nav-link"> <router-link :to="{ name: 'AccountSettingsMain' }">Settings</router-link></a>
                <a class="nav-link" href="blog/classic.html">Sign Out</a>
              </nav>
            </li>

          </ul>
        </section>

      </div>
    </nav><!-- /.navbar -->
</template>
<script>
export default {
  name: 'Navbar',
  data () {
    return {
      msg: 'This is navbar',
      example: 'Testing'
    }
  },
  methods: {
    goToQA () {
      // q-a-main
      this.$router.push({ path: `/questions` })
    }
  }
}
</script>
