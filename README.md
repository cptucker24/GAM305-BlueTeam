# Module Two Team Project Plan

Final Project due: Oct 19th 2025

Google Sheets Traceability Matrix: https://docs.google.com/spreadsheets/d/1PH7QBH8emZVz78BYsZnx3D7BssizTk6aXlcWSa_jMvQ/edit?usp=sharing

Concept: The player acts as some form of antivirus (undetermined) ingested to fight off viruses, harmful bacteria, and other forms of infection within a human's digestive system.

Genre: First-Person Shooter

Game Theme: Inner body workings. Player will play as a body system fighting off viruses (potentially white blood cell? Anti-body? Nano-machine?)

Alpha Stage due: Sept 28th

Beta Stage due: N/A

**Roles**<br>
Lead: Catarena "Cat" Tucker<br>
Programmer: Catarena "Cat" Tucker<br>
Artist: Michael M<br>
Level Design: Tyler B<br>
UI/UX: Anthony (Tony) Domine

**Team Communication Preferences**<br>
Tyler B: Text<br>
Tony D: Text/Voice<br>
Cat T: Text/Voice<br>
Michael M: Text/Voice

**Team Communication Frequency**<br>
As often as necessary via text, schedule out voice calls as needed.

Assigning and reporting of tasks will occur mainly on group chat and traceability matrix. If you need someone in another department to add something, please inform them in the Discord chat and add it to the matrix.

**Features & Assigned Tasks**<br>
Jump pad: Tyler<br>
Pickups (Keycard): Tyler<br>
Minimap & Other UI Elements: Tony<br>
Virus Reproduction: Cat<br>
Miscellaneous: Michael

**Schedule**<br>
Alpha: Due Sept 28th<br>
Tyler: I will have a basic concept for level design, with functional doors, jump pads and a place for the player to move about illustrating the style that we will go for. This will be completed by Sept 24th.

**Play Test**<br>
Tyler: Once the basic test level is built, we can collectively play, test, and provide feedback on each other's roles for changes to be made.

<hr>

**Module Three Project Log - Team Development: QA and Testing Plan**<br>
Prompt: As a game development team, devise a plan for quality assurance and testing your product. Begin by determining a preferred means of communication and a collaborative method to develop your document.<br>

**How will you update the test plan to reflect changes to the game and design document?**<br>
Any and all additional features, mechanics, or assets will be recorded within the Test Plan sheet to consistently reflect the game as is.<br>
**How will bugs be reported and how will the bugs and their changes be tracked over time?**<br>
Communication via Discord and Tracability Matrix under "Test Plan" sheet.

Schedule: Varies amongst members (tasks are completed in free time); congregate as necessary.<br>
Play Test: Following the Demo process, although similar, it requires a more arbitrary approach to intentionally discover bugs & glitches to prevent future errors.<br>
Demo: Members, after each developmental success in their own task, will experiment with their product's functionality as intended.<br>
Code Release: Pertaining to updating files through GitHub, all game modifications - either insertions or deletions - are first uploaded to a separate branch and confirmed with other members before merging it with the Main/Master. (Closest to the Continuous Deployment Strategy?)

**Features to be Tested Checklist (Pass/Fail):**<br>
Level design: Checking for holes in collision of the map, layout design and manueverability.<br>
Keycards: Ensure that they enable the ability to open locked doors.<br>
Jump pad: Applies the right amount of force, consistently no matter how the player is interacting with it.<br>
Sphincter muscle-shaped door: Ensure animation for opening and closing works based on distance (until introducing keycards).<br>
Player Character: Player Character inputs for movement, interactions, and jump.<br>
AI Character: Ensure AI Character is set up with Behavior Tree.<br>
AI Character Respawn: Ensure AI Character can respawn after a certain period due to losing health.<br>
UI Elements: Running game from start (menu), then interacting with the world (damage for healthbars, and minimap on screen to track enemies/world).
<br><br>
**Pickups:**<br>
Keycards: Complete(TB)<br>

**Module Four Project Log - Team Reflection**<br>
**What parts of the testing process did the team perceive to go well?**<br>

**How were bugs identified and corrected?**<br>
While testing a simple animation for the doors, it would open initially when entering range, but soon stop working, then work again. I realized that I was trying to made two separate animative functions because of a previous, minor issue (so I was testing what went wrong): one for opening when the player enters the range, and one for closing when the player leaves. After discovering the initial problem, I scrapped the latter and connected both events to the same Timeline function node. One event played it forward, and the other played it backward.
**In terms of the QA and testing process, what would you do differently to improve the process?**<br>

**What tools (chosen in Module Two) did you find successful in the development of your Alpha project? Why?**<br>

**Were there any tools or techniques that you did not find helpful in the success of your project development? Why?**<br>

**How did the team approach to the initial analysis of the game design document contribute to the decision to use these tools and techniques?**<br>
