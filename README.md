# Module Two Team Project Plan

Final Project due: Oct 19th 2025

Google Sheets Traceability Matrix: https://docs.google.com/spreadsheets/d/1PH7QBH8emZVz78BYsZnx3D7BssizTk6aXlcWSa_jMvQ/edit?usp=sharing

Concept: The player acts as some form of antivirus (undetermined) ingested to fight off viruses, harmful bacteria, and other forms of infection within a human's digestive system.

Genre: First-Person Shooter

Game Theme: Inner body workings. Player will play as a body system fighting off viruses (potentially white blood cell? Anti-body? Nano-machine?)

Alpha Stage due: Sept 28th

Beta Stage due: N/A

## Roles<br>
Lead: Catarena "Cat" Tucker<br>
Programmer: Catarena "Cat" Tucker<br>
Artist: Michael McCallister<br>
Level Design: Tyler Banes<br>
UI/UX: Anthony (Tony) Domine

## Team Communication Preferences<br>
Tyler B: Text<br>
Tony D: Text/Voice<br>
Cat T: Text/Voice<br>
Michael M: Text/Voice

## Team Communication Frequency<br>
As often as necessary via text, schedule out voice calls as needed.<br>
Assigning and reporting of tasks will occur mainly on group chat and traceability matrix. If you need someone in another department to add something, please inform them in the Discord chat and add it to the matrix.

## Features & Assigned Tasks<br>
Jump pad: Tyler<br>
Pickups (Keycard): Tyler<br>
Minimap & Other UI Elements: Tony<br>
Virus Reproduction: Cat<br>
Miscellaneous: Michael

## Schedule<br>
Alpha: Due Sept 28th<br>
Tyler: I will have a basic concept for level design, with functional doors, jump pads and a place for the player to move about illustrating the style that we will go for. This will be completed by Sept 24th.

## Play Test<br>
Tyler: Once the basic test level is built, we can collectively play, test, and provide feedback on each other's roles for changes to be made.

<hr>

# Module Three Project Log - Team Development: QA and Testing Plan<br>
**Prompt:** As a game development team, devise a plan for quality assurance and testing your product. Begin by determining a preferred means of communication and a collaborative method to develop your document.<br>

## How will you update the test plan to reflect changes to the game and design document?<br>
Any and all additional features, mechanics, or assets will be recorded within the Test Plan sheet to consistently reflect the game as is.<br>
## How will bugs be reported and how will the bugs and their changes be tracked over time?<br>
Communication via Discord and Tracability Matrix under "Test Plan" sheet.

**Schedule:** Varies amongst members (tasks are completed in free time); congregate as necessary.<br>
**Play Test:** Following the Demo process, although similar, it requires a more arbitrary approach to intentionally discover bugs & glitches to prevent future errors.<br>
**Demo:** Members, after each developmental success in their own task, will experiment with their product's functionality as intended.<br>
**Code Release:** Pertaining to updating files through GitHub, all game modifications - either insertions or deletions - are first uploaded to a separate branch and confirmed with other members before merging it with the Main/Master. (Closest to the Continuous Deployment Strategy?)

## Features to be Tested Checklist (Pass/Fail):<br>
**Level design:** Checking for holes in collision of the map, layout design and manueverability.<br>
**Keycards:** Ensure that they enable the ability to open locked doors.<br>
**Jump pad:** Applies the right amount of force, consistently no matter how the player is interacting with it.<br>
**Sphincter Muscle-shaped Door:** Ensure animation for opening and closing works based on distance (until introducing keycards).<br>
**Player Character:** Player Character inputs for movement, interactions, and jump.<br>
**AI Character:** Ensure AI Character is set up with Behavior Tree.<br>
**AI Character Respawn:** Ensure AI Character can respawn after a certain period due to losing health.<br>
**UI Elements:** Running game from start (menu), then interacting with the world (damage for healthbars, and minimap on screen to track enemies/world).<br>

## Pickups:<br>
**Keycards:** Complete(TB)<br>

<hr>

# Module Four Project Log - Team Reflection<br>

## What parts of the testing process did the team perceive to go well?<br>
**Tyler:** General testing seemed to go fine in my opinion. We are bound to find bumps in the road but overall, we got things fixed up just fine.<br>
**Michael:** There seemed to be little to no issues regarding merging branches. Similarly, all the desired features that have yet been implemented function properly and as desired.<br>
**Tony:** Similar thoughts, as testing itself appears to have gone fairly well in finding things that either still need to be implemented or fixed for future release.<br>
**Cat:** Testing seems to be going well so far. Everything is looking good so far.<br>

## How were bugs identified and corrected?<br>
**Michael:** While testing a simple animation for the doors, it would open initially when entering range, but soon stop working, then work again. I realized that I was trying to made two separate animative functions because of a previous, minor issue (so I was testing what went wrong): one for opening when the player enters the range, and one for closing when the player leaves. After discovering the initial problem, I scrapped the latter and connected both events to the same Timeline function node. One event played it forward, and the other played it backward.<br>
**Tyler:** While testing out and building the level design, I ran into an issue where nothing had collision detection. This was solved by finding the setting that determines the collision type. Normally, this defaults to simple collision, but was generating all geometry to no collision. Simple fix but a good experience in learning to not expect the engine to always behave the same way every time. Furthermore, another issue came from the character rebuilds that were done. Simple relinks to fix most issues but building the project failed because the old file was still present. I assumed that when the previous file was deleted in engine, it deleted it off my HDD as well but I think it remained on the project.<br>
**Tony:** When testing earlier in the week, there were several errors that popped up at one point, only to discover the main issue was with some variables becoming un-linked or needing to be reset. Currently working on implementing and creating a minimap has provided a few challenges, while not a bug (yet), I realized if I were to put what I have in right now, it may break or create more problems than it would help the project overall while I am working to understand & make it work properly. Currently does not display the map or enemies as it should, which will be my main focus int he upcoming week(s). <br> 
**Cat:** The only error that I ran into this week with testing is that the playerchar I created disappeared somehow. I managed to make another playerchar, but we ran into a small bump with the old playerchar. Luckily, my team was able to get it fixed with no issues.<br>

## In terms of the QA and testing process, what would you do differently to improve the process?<br>
**Tyler:** More organization and defined roles and expectations within the team so we all test the same things at different phases. Different hardware will give us different results and that is important for testing.<br>
**Cat:** I would try to incorporate test passes for each blueprint, such as if the AI respawns after a certain amount of time, or if the hit box is working correctly on both the player character and AI character.<br>

## What tools (chosen in Module Two) did you find successful in the development of your Alpha project? Why?<br>
**Tyler:** I still prefer the matrix that we set up in the beginning but find that it was significantly under utilized.<br>
**Tony:** During the development, I also found using the traceability matrix helped organize thoughts and see what needs to be done on my end. This along with many past and newly found tutorial videos, have helped remember/implement different features into the project.<br>
**Cat:** I prefer using the Traceablility Matrix to keep up with all testing and phases of development, as well as utilizing the tutorial videos from my previous classes and those that my teammates have provided to assist me.<br>

## Were there any tools or techniques that you did not find helpful in the success of your project development? Why?<br>
**Tyler:** The ReadMe. The information in here is not readily available and is generally not convienant to access.<br>
**Cat:** I have the most issues with GitHub on my PC. I'm unable to access the website to do my work in Unreal Engine. I have the desktop version on my PC, but that still doesn't give me everything that I need to work properly. I have to use my laptop just to edit the README.<br>

## How did the team approach to the initial analysis of the game design document contribute to the decision to use these tools and techniques?<br>
**Tyler:** I think mainly it was breaking down the requirements of the end project and deciding what we need from there then speaking about what we did in previous classes to stay organized.<br>
**Tony:** We certainly communicated clearly with one another about our strengths and how we might tackle the project; which I think helped quite a bit in getting us on track and working on it quickly.<br>
**Cat:** I believe we all were able to communicate how we felt about each role, and even offered assistance on certain things, if assistance is needed.<br>
**Michael:** We consistently communicate over the discord channel about each little step everyone of us take; whetehr it's adding a new feature, providing test results, or even just mentioning ideas. Doing so allowed us to decide what would be implemented and the tasks in which we were assigned.<br>

<hr>

# Module Five Project Log - Team Reflection

## What parts of the plan did the team perceive to go well in relation to the last stage evaluation?<br>
**Tyler:** Development of the level design went well. I spent a lot more time making the level flow and used lighting to help direct the player. I still have a bit more to do to meet minimum requirements for the final submission.<br>
**Michael:** Pertaining to the build's textures, I was able to create a "Master Material" that allowed any instance derived from it to be modified in every aspect. It has a lot of benefits and allows each member to do their own thing based on a single material blueprint.<br>

## What parts of the plan did the team perceive to go wrong in relation to the last stage evaluation?<br>
**Tyler:** We have a lot more to implement and time is closing in on us. I feel like a lot more could have been done earlier so we can balance out for the final product better.<br>
**Michael:** Since the integration from Quixel Bridge to Fab, I have had fewer options to use free meshes and textures for the levels and assets. While I was able to make do for some walls, floors, and whatnot, I am still searching for good character/enemy meshes appropriate for the build.<br>

## How were the previous evaluations integrated into this latest stage?<br>
**Tyler:** If this is referring to feedback provided, I listened by changing the entire level and making it more directed and easier to navigate. Otherwise, most things were implemented from the previous installment. It was just moved around a bit.<br>

## What would you do differently to improve the collaboration or development process?<br>
**Tyler:** I'd like a more detailed gameplan for things. More definitive and cohesive vision between everyone earlier on but given the time frame of the class, it isn't bad.<br>
**Michael:** The biggest problem, I think, is time and general availability. Each week someone has something going on which deducts time that could be used for development. As long as we can all utilize our time and plan our tasks (similar to Tyler's response), we could continue efficiently.<br>

## Were there any tools or techniques that you did not find helpful in the success of your project development? Why?<br>
**Tyler:** I still find the matrix to be underutilized and the ReadMe to be too crowded to find information quickly.<br>

## Identify the completed stage of development of the intended Beta and address the project schedule to meet Final Release development deadline.<br>
**Tyler:** I would say we are half way between Alpha and Beta. If Beta is defined as having assets, mechanics and level(s) fully defined, then we aren't quite there. We are close to Beta, however. For the schedule, we have about 2 weeks to finish everything up.<br>
**Michael:** I agree we are about halfway, more or less, of what we are trying to accomplish in terms of playability and it must be finsihed within 2 more weeks.
