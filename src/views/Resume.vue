<template>
  <div>
    <h1>Resume</h1>

    <div class="paragraph">
        Hello There! <br />
        I'm <strong>Daud Zaidi</strong> an enthusiastic game designer with a burning
        passion for creating immersive gaming experiences.<br/>
        I'm constantly on the lookout for ways to expand my skills and stay in
        touch with the latest trends and technologies. I believe that keeping
        an open mind and embracing new ideas is crucial in this dynamic
        industry.<br/>
        Let's join forces and create captivating experiences that bring joy to
        players worldwide!
        Feel free to <router-link to="/contact">contact me</router-link> if you would like to know more!
        <div style="margin-top:20px; margin-bottom:20px;">
            <a class="download-link" href="d/resume-en.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Download as PDF 🇬🇧</a>
            <a class="download-link" href="d/cv-fr.pdf" target="_blank"><i class="fa fa-download fa-lg fa-fw"></i> Télécharger en PDF 🇫🇷</a>
            <div style="clear:both"></div>
        </div>
    </div>
    <div class="photo">
      <img src="img/DaudZaidi.png" alt="Photo of Me" />
    </div>

    <div style="clear:both"></div>

    <div class="full-content">
        <h2>Work experience</h2>

        <h3>Game Designer - GeniTeam Solutions</h3>
        <h4>August 2022 - February 2024</h4>
        <ul>
            <li>Participated in 3+ Design Sessions with management for improving existing games KPIs</li>
            <li>Prepared Game Design Documents for 5+ new titles.</li>
            <li>Crafted 120+ levels for 3 level based games.</li>
            <li>Creating UX frameworks together with UI Artists for 5+ games.</li>
            <li>Published 3+ successful games that surpassed set KPIs</li>
            <li>Led the Development, Art and Animation Teams for 5+ new titles</li>
        </ul>



        <div class="tech-stack">Unity, Figma, Miscrosoft Office, Illustrator, Machinations, Game Analytics, ... </div>

        <h2>Skills</h2>

        <div class="skill-set">
            <h3>Game Design</h3>
            <SkillRate name="Mechanics Design" :rate="5" />
            <SkillRate name="Level Design" :rate="5" />
            <SkillRate name="Puzzle Design" :rate="4" />
            <SkillRate name="Narrative Design" :rate="4" />
            <SkillRate name="Economy Design" :rate="3" />
        </div>

        <div class="skill-set">
            <h3>Game Development</h3>
            <SkillRate name="C# Programming" :rate="4" />
            <SkillRate name="Unity Engine" :rate="4" />
            <SkillRate name="Architecture Design" :rate="3" />
            <SkillRate name="Game Mechanics" :rate="3" />
        </div>
        <div style="clear:both" />

        <h2>Education</h2>

        <h3>Master Studies</h3>
        <h4>Masters in Entrepreneurship (2024 - ongoing) </h4>
        <div>Specialty in bullying and fighting (58 wins, 58 K-O, 0 losses)</div>

        <h3>Bachelor Studies</h3>
        <h4>Bachelor in Business Administration (2016 - 2020) </h4>
        <div>Graduated with an A Grade</div>
        
        <h2>Languages</h2>

        <h3>English</h3>
        <div>Fluent - 8.5 IELTS bands</div>

        <h2>Hobbies...</h2>
        <div>
            <h3>I ❤️ To Game</h3>
            <div>My favorite game is Dota 2 and I can play it for hours long! Apart from Dota, I enjoy story mode games
            such as Last of Us, God Of War, and Red Dead Redemption 2!</div>

            <h3>I 🧡 To Read</h3>
            <div>My favorite category of books are fiction. I specially enjoyed reading the The Lord of The Rings, and Harry Potter series!</div>

            <h3>I 💛 To Play Basketball</h3>
            <div>Whenever I can, I go out with firends for a basketball session!</div>

        </div>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import SkillRate from "@/components/SkillRate.vue";

export default Vue.extend({
  name: "Resume",
  components: {
    SkillRate,
  },
});
</script>

<style scoped>
h2 {
  font-weight: 100;
  font-size: 2em;
  margin: 0px;
  padding: 0px;
  padding-top: 50px;
}
h3 {
  font-weight: 100;
  font-size: 1.6em;
  margin: 0px;
  padding: 0px;
  padding-top: 30px;
}
h4 {
  font-weight: 100;
  font-size: 1.3em;
  margin: 0px;
  padding: 0px;
  padding-top: 15px;
  font-style: italic;
}

.paragraph {
  max-width: 700px;
}

.download-link {
  float:left;
  margin-right: 50px;
}

.full-content div {
  max-width: 800px;
}

.skill-set h3 {
  padding-bottom: 10px;
}

.photo img {
  height: 300px;
  width: 300px;
}

.tech-stack {
  font-style: italic;
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
    padding: 30px;
    padding-left: 80px;
  }

  .skill-set {
    float: left;
    padding-right: 60px; 
  }
}
</style>