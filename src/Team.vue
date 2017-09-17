<template>
    <div class="team-wrapper" :style='{ backgroundImage: `url(${team.logoUrl})` }'>
      <div class="nice-list">
        <ul>
          <li class="item">
            <p>{{team.name}}</p>
          </li>
          <li>
            <p>Score: {{team.weekScore}}</p>
          </li>
          <li>
            <p>Total Score: {{team.totalScore}}</p>
          </li>
        </ul>
      </div>
  </div>
</template>

<style>

.team-wrapper {
  border-radius: 2px;
  background-size: cover;
  background-position: center;
  width:auto;
  height: 250px;
  padding: 10px;
}

.item {
  display: inline-block;
}

.nice-list ul {
  margin: 10px 20px;

  border-radius: 4px;
  list-style:none; 
  background-color:rgba(51, 51, 51, 0.7);
  padding: 8px 0;
  box-shadow:5px 10px 10px #333333; 

}

.nice-list ul li  {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  font-size:18px;  
  display:block; 
  height:24px; 
  text-decoration:none; 
  color:#bfe1f1; 
  margin: 10px 5px;
  border-radius: 4px;
  
}

.nice-list ul li :hover {  
  -moz-transform:rotate(2deg); 
  -moz-box-shadow:10px 10px 20px #000000;
  -webkit-transform:rotate(2deg); 
  -webkit-box-shadow:10px 10px 20px #000000;
  transform:rotate(2deg); 
  box-shadow:10px 10px 20px #000000; 
  border-radius: 2px;
}

.nice-list ul li p {
  margin: 10px;
  padding: 2px 10px;
 }

</style>

<script>
export default {
  name: 'TeamComponent',
  data () {
    return {
      team: {
        name: "Offensive Fowlers",
        weekScore: 44,
        totalScore: 400,
        logoUrl: "http://i.imgur.com/xQb6fteb.jpg"
      }
    }
  }
}
</script>


