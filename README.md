<img src="https://doki.assets.unthrottled.io/misc/best_girl.png" />

<br/>

<details>
  <summary>Facts</summary>
  
```
__________                    ___________                  
\____    /___________  ____   \__    ___/_  _  ______      
  /     // __ \_  __ \/  _ \    |    |  \ \/ \/ /  _ \     
 /     /\  ___/|  | \(  <_> )   |    |   \     (  <_> )    
/_______ \___  >__|   \____/    |____|    \/\_/ \____/     
        \/   \/                                            
__________                 __      ________.__       .__   
\______   \ ____   _______/  |_   /  _____/|__|______|  |  
 |    |  _// __ \ /  ___/\   __\ /   \  ___|  \_  __ \  |  
 |    |   \  ___/ \___ \  |  |   \    \_\  \  ||  | \/  |__
 |______  /\___  >____  > |__|    \______  /__||__|  |____/
        \/     \/     \/                 \/                
```
</details>


<details>
  <summary>My 3x3</summary>
  <img alt="3x3" src="./3x3.png"/>
  
  #TeamNino #TeamOnoderaNasaki #TeamHimawari
</details>

<details>
  <summary>Bio.ts</summary>
 
 ```typescript
class Alex extends Weeb implements Hacker, Athlete {
  startWorkingDay() {
    while (shouldContinue()) {
      学习中文(); // TODO: look into finding where memory leaks are....
      const currentProject = this.getCurrentProject();
      continueWorkingOn(currentProject);
      perform(this.getCurrentWorkout());
      perform(getDayJob());
      perform(getWalkingRoute());
      continueWorkingOn(currentProject);
      watch(this.pickAnime());
      question(getCurrentLifeChoices());
      sleep(this.getDesiredHoursOfSleep());
    }
  }

  startRestDay() {
    eat(findFood());
    const animeForTheDay = this.pickAnime();
    watch(animeForTheDay);
    perform(getWalkingRoute())
    watch(animeForTheDay);
    sleep(this.getDesiredHoursOfSleep());
    // TODO: Need to find more hobbies.
  }

  private favoriteLanguages = ['TypeScript', 'Kotlin'];
  private getCurrentProject(): Project {
    const buggyProjects = getMaintainedOSSProjects()
      .filter(project => 
          project.reportedBugs()
            .filter(bug => !isFeature(bug))
            .some(bug => doICareEnoughToFix(bug))
      );
    if(!!buggyProjects.length) {
      return new BugFixProject(buggyProjects);
    } else if(!this.hasEnoughAnimeGirlThemes()) {
      return new ExasterbateAnimeAddictionProject();
    }
    const chosenLanguage = pickRandom(this.favoriteLanguages);
    return new RandomProject(chosenLanguage, pickRandomTopic(chosenLanguage));
  }

  private hasEnoughAnimeGirlThemes() {
    return isStillWeeb() && getDurationFromLastBuiltTheme()
      .isGreaterThan(Duration.of(30, DAYS));
  }

  private getCurrentWorkout(): Workout {
    switch (getCurrentDay()) {
      case Days.MONDAY: return Workout.LEGS;
      case Days.TUESDAY: return Workout.PUSH;
      case Days.WEDNESDAY: return Workout.PULL;
      case Days.THURSDAY: return Workout.SHOULDERS;
      case Days.FRIDAY: return Workout.CARDIO;
      default: return Workout.RECOVERY;
    }
  }

  private favoriteAnimeGenres =
    new Set(['Romance', 'Slice of Life', 'Isekai', 'Comedy']);
  private pickAnime(): Anime {
    while (true) {
      const nextAnime = pickRandomAnime();
      const genre = nextAnime.genre;
      if (this.favoriteAnimeGenres.has(genre) ||
        (isTrash(nextAnime) && isEcchi(nextAnime))) {
        return nextAnime;
      }
    }
  }

  private getDesiredHoursOfSleep() {
    return isWeekday() ? 7.5 : pickRandomNumberBetween(7, 10);
  }
}
```

 
</details>



