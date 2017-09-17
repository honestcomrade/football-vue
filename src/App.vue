<template>
  <div id="app">
    <div class="msg-container">
      <h2>{{msg}}</h2>
    </div>
    <nav>
      <ul>
        <li>
          <a href="http://games.espn.com/ffl/leagueoffice?leagueId=262704&seasonId=2017" target="_blank">TEAM</a>
        </li>
        <li>
          <a href="http://games.espn.com/ffl/leagueoffice?leagueId=262704&seasonId=2017" target="_blank">LEAGUE</a>
        </li>
        <li>
          <a href="https://github.com/honestcomrade" target="_blank">SUPPORT</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      msg: 'Welcome back to your team, Jes!'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

html {
  background-image: url(./assets/banner.jpg);
  background-size: cover;
  background-position: center;
  width: 100%;
  height: 100%;
}

h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}

nav {
  width: 100%;
  background-color: rgb(250, 250, 243);
  position: absolute;
  bottom: 0;
  left: 0;
}

nav a {
  font-weight: 500;
  text-decoration: none;
}

.msg-container{
  color: seashell
}

</style>
