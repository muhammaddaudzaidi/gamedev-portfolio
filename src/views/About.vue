<template>
  <div style="margin-bottom: 80px;">
    <h1>Hello!</h1>

    <div class="paragraph">
      <div>
        I'm <strong>Daud Zaidi</strong>, a game designer & developer!<br/>
        I have 18 months of experience as a <strong>Game Designer</strong> while I also participated in game jams as a <strong>Game Developer</strong>.
      </div>

      <div style="margin-top: 20px;">
          During my career as a Game Designer, I have worked on four mobile games that can be viewed from <strong><router-link to="/game-projects">Published Games</router-link></strong> section.<br/>
          
          In addition, I have also participated in <strong><router-link to="/other-projects">Game Jams</router-link></strong> where I was both a programmer and a designer for my teams.<br />
          
          You can also check out my <strong><router-link to="/resume">Resume</router-link></strong> to know better about my skills and achievements!<br />
      </div>
      
      <div style="margin-top: 40px;">Currently, I am on a lookout for a role in <strong>Game Design</strong>. If you like my profile, you can reach me at <strong><a href="mailto:sydaudzaidi@gmail.com">sydaudzaidi@gmail.com</a></strong> or <strong><router-link to="/contact">through here</router-link></strong>.</div>
    </div>

    <div class="photo">
      <img src="img/Daud Zaidi.png" alt="Avatar of Daud" /> 
    </div>

    <div style="clear:both"></div>

  </div>
</template>

<style scoped>
.paragraph {
  max-width: 700px;
  margin-bottom: 20px;
}

.photo {
  margin-top: 50px;
  text-align: center;
}

@media only screen and (min-width: 620px){
  .paragraph {
    float: left;
  }

  .photo {
    float: left;
    padding: 10px;
    padding-left: 80px;
  }
}

</style>