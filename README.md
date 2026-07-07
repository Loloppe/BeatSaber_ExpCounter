# ExpCounter

Beat Saber Counters+ plugin for BeatLeader XP System.  
Display how much XP you would gain while playing.  

This plugin is only accurate if:
- 60% of the notes were cut properly
- Map has more than 10 notes
- Not playing in practice mode

XP system reward 9 XP per second of active gameplay.  
Final result is affected by the player accuracy during score submission.  
XP calculation is: XP * Duration * Accuracy  
Accuracy curve can be found here: https://github.com/Loloppe/BeatSaber_ExpCounter/blob/8841dca17aafcca449bf17c5992f26cbae6fd2bc/ExpCounter/Utils/ExperienceUtils.cs#L9  
The accuracy curve is very lenient. The player only need to maintain 95% accuracy to gain 100% XP (ceiling). 30% accuracy and under give 30% XP (floor).
