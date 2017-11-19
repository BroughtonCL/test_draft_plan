# test_draft_plan
# Test Plan for: CyberBlitz by The Waffle Group (NVC GAME 2359 FAll 2017)

## Summary Information
### Summary of CyberBlitz
The Waffle Group has created a 1 to 4 player game based on the game of Dodge Ball. This game targets the casual to intermediate gamer and depicts a futuristic game of Dodge Ball in one of three arenas.

The player or players control a selected 'bot' to get a ball, retreat to the attack area and throw the ball at the opponent. Avatars in the game not controlloed by the user or users will get controlled by the computer (AI). The player or players can select from one of four avatars on either the Red team or the Blue team. The player can chose either Bao - a Panda playing bot, Cole a more traditional bot, Maya or Girl bot and Unit-Y a bat playing bot. The players can cose to play with one, all or any combination of the following balls: Neon Ball the default ball, fastest and simplist, the Bomb Ball slower but will explode "killing all the opposition" in an area, the Freeze Ball that stops the opposition in an area for a shorttime, the Asian Ball that splits into two balls (Ying and Yang) and the homing ball that will chase players. The chosen balls will get 'spawned' randomly in the center of the court to replace thrown balls used in game play.

Play will take place on one of three courts: Neon Arena futuristic arena somewhat like Tron, Crystal Cave ina a cave with large crystals and other cave objects and Asian Arena a futureinstic Dojo that flies over a future asian city.

### Environment/User Community (Identify user community and where testing will be performed)
The first version of the game wuill run on Windows 7 and 10 in a standalone environment.  The tests will occure on 'builds' downloaded and installed on the test machines.  The Waffle Group used the Unity game engine to develop this application and as such provides teh drivers to run the game in under Windows 7 (professional) and Windoes 10 (Home Edition).

The testing will occur ina class room environment using PCs running the Window operating system and personal PCs of teh testers to test under Windows 10 in a standalone environment.

### Test Objectives (State objectives to be accomplished by testing)
We plan to meet the following objectives:
1.  QA on all the major functions of the application
2.  Provide feed back on gameplay objectives
3.  Document and provide feed back on all bugs found.
4.  Test a late Alpha build and a Beta Build (Time permitting before last report deadline).

We plan to run the following test cases on each build teseted:
### Test Case 1 - "smoke" test of the CyberBlitz under the Windows 7 operating system
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID: 
  * 001
* Test Case Name:
  * Test Case 001 - "smoke" test of the CyberBlitz under the Windows 7 operating system
* Component: 
  * The build that tests this version of the game on Windows 7 in a standalone environment.
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * Travis Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Install, Load Start Install game on PC
  * Main Menu (02_MainMenu) Main Menu and all buttons function
  * Game Setup (03_GameSetup) Player selection and Match Settings buttons work correctly
  * SA Neon Arena (04_NeanArena) Game plays on this arena
  * Lumnos Cave Arena (05_CaveArena) Game plays on this arena
  * Asian Arena (06_AsianArena) Game plays on this arena
* Test Description/Purpose:
  * Install and run the game from the provided 'build' file folder
  * Main Menu test the button functionality ab navigation of this scene
  * Game Setup - This scene consists of two full sized panels
    * First "Chooze Your Blitzer" to imput palyer setup options
    * Second "Match Settings" to enter match options.
  * SA Neon Arena (04_NeanArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.
  * Lumnos Cave Arena (05_CaveArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.
  * Asian Arena (06_AsianArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.

* Pre-Test Conditions:
  * The first version of the game wuill run on Windows 7 and 10 in a standalone environment.  The tests will occure on 'builds' downloaded and installed on the test machines.  The Waffle Group used the Unity game engine to develop this application and as such provides the drivers to run the game in under Windows 7 (professional).

The testing will occur in a class room environment using PCs running the Window operating system.
#### Test Steps: 
##### Install, Load Start Install game on PC
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Install game | Zip file extracts without errors - data fiela nd exe in taget location | |			
| 2 | Sart/load game | Double click on exe -after splash screen ask user for display options then starts game load scene | |		
| 3 | Load->Main Menu | Main Menu laods after 5 seconds or user clich (which happens first)| |
| Sart/load game | Double click on exe -after splash screen ask user for display options then starts game load scene |

#####  Main Menu (02_MainMenu) Main Menu and all buttons function
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Play       | Go to the game setup scene (03_GameSetup) Player setup Panel | |			
| 2 | Quick Play | Go to the default scene (Cave Arena) and play the default match | |			
| 3 | Controls   | Drops a "Help" panel that explains the controls | |			
| 4 | Settings   | Drops a Settings panel that allows the user to change some settings | |			
| 5 | Credits    | Drops a panel with game credits and copyrights | |			
| 6 | Quit       | Exits the application | |			
##### Game Setup (03_GameSetup) Player selection buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Players shown            | Display the default number of players as a function of detected controllers | |			
| 2 | Click on Player header   | Change weather the avatar get controlled by the user or the computer | |			
| 3 | Click on Players picture | Change the player's avatar. | |			
| 4 | Select drop down         | Change the controller used to control the avatar | |			
| 5 | Click on 2 or 4 players  | Change between two and for players | |			
| 6 | Click on Main Menu       | Go back to the Main Menu | |			
| 7 | Click on Next            | Go to the Match Settings panel | |			
##### Game Setup (03_GameSetup) Match Settings buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Display | Display the default arena, balls and match time.       | |			
| 2 | Click on balls | Allow the user to select or deselect the match balls | |			
| 3 | Click on time arrows | Allow the user to increase or decrease the match time | |			
| 4 | Click on Arena | Allow the user to select the arena to play | |			
| 5 | Click on Blitz | Go play game in selected arean | |			
| 6 | Click on Back | Go back to the player setup panel | |			
##### SA Neon Arena (04_NeanArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Neon Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
##### Lumnos Cave Arena (05_CaveArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Cave Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
##### Asian Arena (06_AsianArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Asian Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
#### Overall Test Status:

### Test Case 2 - "smoke" test of the CyberBlitz under the Windows 10 operating system
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID: 
  * 002
* Test Case Name:
  * Test Case 002 - "smoke" test of the CyberBlitz under the Windows 10 operating system
* Component: 
  * The build that tests this version of the game on Windows 7 in a standalone environment.
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * Travis Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Install, Load Start Install game on PC
  * Main Menu (02_MainMenu) Main Menu and all buttons function
  * Game Setup (03_GameSetup) Player selection and Match Settings buttons work correctly
  * SA Neon Arena (04_NeanArena) Game plays on this arena
  * Lumnos Cave Arena (05_CaveArena) Game plays on this arena
  * Asian Arena (06_AsianArena) Game plays on this arena
* Test Description/Purpose:
  * Install and run the game from the provided 'build' file folder
  * Main Menu test the button functionality ab navigation of this scene
  * Game Setup - This scene consists of two full sized panels
    * First "Chooze Your Blitzer" to imput palyer setup options
    * Second "Match Settings" to enter match options.
  * SA Neon Arena (04_NeanArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.
  * Lumnos Cave Arena (05_CaveArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.
  * Asian Arena (06_AsianArena) - show camera animations, appropriate UI, show match time move avatars in response to player input.

* Pre-Test Conditions:
  * The first version of the game wuill run on Windows 10 in a standalone environment.  The tests will occure on 'builds' downloaded and installed on the test machines.  The Waffle Group used the Unity game engine to develop this application and as such provides the drivers to run the game in under Windows 10 (Home edition).

The testing will occur in a class room environment using PCs running the Window operating system.
#### Test Steps: 
##### Install, Load Start Install game on PC
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Install game | Zip file extracts without errors - data fiela nd exe in taget location | |			
| 2 | Sart/load game | Double click on exe -after splash screen ask user for display options then starts game load scene | |		
| 3 | Load->Main Menu | Main Menu laods after 5 seconds or user clich (which happens first)| |
| Sart/load game | Double click on exe -after splash screen ask user for display options then starts game load scene |

#####  Main Menu (02_MainMenu) Main Menu and all buttons function
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Play       | Go to the game setup scene (03_GameSetup) Player setup Panel | |			
| 2 | Quick Play | Go to the default scene (Cave Arena) and play the default match | |			
| 3 | Controls   | Drops a "Help" panel that explains the controls | |			
| 4 | Settings   | Drops a Settings panel that allows the user to change some settings | |			
| 5 | Credits    | Drops a panel with game credits and copyrights | |			
| 6 | Quit       | Exits the application | |			
##### Game Setup (03_GameSetup) Player selection buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Players shown            | Display the default number of players as a function of detected controllers | |			
| 2 | Click on Player header   | Change weather the avatar get controlled by the user or the computer | |			
| 3 | Click on Players picture | Change the player's avatar. | |			
| 4 | Select drop down         | Change the controller used to control the avatar | |			
| 5 | Click on 2 or 4 players  | Change between two and for players | |			
| 6 | Click on Main Menu       | Go back to the Main Menu | |			
| 7 | Click on Next            | Go to the Match Settings panel | |			
##### Game Setup (03_GameSetup) Match Settings buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Display | Display the default arena, balls and match time.       | |			
| 2 | Click on balls | Allow the user to select or deselect the match balls | |			
| 3 | Click on time arrows | Allow the user to increase or decrease the match time | |			
| 4 | Click on Arena | Allow the user to select the arena to play | |			
| 5 | Click on Blitz | Go play game in selected arean | |			
| 6 | Click on Back | Go back to the player setup panel | |			
##### SA Neon Arena (04_NeanArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Neon Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
##### Lumnos Cave Arena (05_CaveArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Cave Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
##### Asian Arena (06_AsianArena) Game plays on this arena
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Scene Loads | Start with a camera animation and end focused on the playing surface in the Asian Arena       | |			
| 2 | Game Display | Display the proper UI for the number of players | |			
| 3 | Game Display | Start the match and match clock | |			
| 4 | User input - Keyboard mouse or controller | Play the game | |			
| 5 | Esc key or Pause button | Pause the game and drop a Pause panel that allows (Resume, Main Menu, Controls andSettings) | |			
| 6 | Time == 0:00 | Display score and game over panel at end of match (Main Menu, and Play again) | |			
#### Overall Test Status:

### Test Case 3 - functional test of the game install, run and load on the user's PC (Scenes 00_Persistent, 01_Load and 02_MainMenu))
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/17
##### Ver. 0.8
* Test Case ID:
  * 003
* Test Case Name:
  * 003 - Functional test of the game install, run and load on the user's PC (Scenes 00_Persistent and 01_Load)
* Component: 
  * Game start and load scenes, 00_Persistent and 01_Load
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * Travis Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * The game loads and starts correctly
  * The user can make perform desired actions
  * The user can select the avatar, controller and game mode desired (Choose Your Blitzer)
  * The user can select the arena, match time and dodge balls desired (Match Settings)
* Test Description/Purpose:
  * Perform detailed functional tests on the first four scenes of the Cyber Blitz game, scenes: 00_Persistent and 01_Load.  
  * Install and run the game from the provided 'build' file folder
* Pre-Test Conditions:
  * Current build of the game wuill run on Windows 7 and 10 in a standalone environment. 
#### Test Steps: 
##### Install, Load Start Install game on PC
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Double click on exe icon |  The game startup screen appears, then the a splash screen asks user for display options | |
| 2 | Check Windowed then Play | The game playes in a window | |
| 3 | Check Full screen then Play | The game playes full screen | |
| 4 | Check Smaller resolution then Play | The game playes in a window sized to the selected resolution | |
| 5 | Wait | Main Menu loads after 5 seconds | |
| 6 | Click Splash screen display options | Display trasitions to MainMenu on click | |
### Test Case 4 - functional test of the Main Menu (scene 02_MainMenu) when loaded from game start testing both keyboar-mouse and game controller input
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/17
##### Ver. 0.8
* Test Case ID:
  * 004
* Test Case Name:
  * 004 - Functional test of the MainMenu (Scene 02_MainMenu)
* Component: 
  * Game Main Menu scene, 02_MainMenu
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * Travis Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * The user can make perform desired actions on the menu: Play, Quick Play, Controls, Settings, Quit and Credits
* Test Description/Purpose:
  * Perform detailed functional tests on Cyber Blitz game 02_MainMenu.
  * Main Menu test the button functionality and navigation of this scene
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * Game started normally and now displays the main menu.
  * The PC has both a game controller and mouse attached.
#### Test Steps: 
#####  Main Menu (02_MainMenu) Main Menu and all buttons function
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Click 'Play' | Display transitions to the game setup scene (03_GameSetup) "Choose Yout Blitzer" panel | |			
| 2 | Click 'Quick Play' or press controller A | Go to the default scene (Cave Arena) and play the default match | |			
| 3 | Click 'Controls' or press controller A | Drops a 'Help' panel that explains the controls | |
| 4 | Click on 'Close' or press controller A | 'Help' panel raise from screen | |
| 5 | Click 'Settings' or press controller A | Drops a Settings panel that allows the user to change some settings | |
| 6 | Click on 'Close' or press controller A | 'Settings' panel raise from screen | |
| 7 | Click 'Credits' or press controller A | Drops a panel with game credits and copyrights | |	
| 8 | Click on 'Close' or press controller A | 'Settings' panel raise from screen | |
| 9 | Click 'Quit' or press controller A | Exits the application | |			
#### Overall Test Status:

### Test Case 5 - functional test of the Main Menu (scene 02_MainMenu) when loaded from a paused game and game setup (loaded from scenes  testing both keyboar-moause and game controller input
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 005
* Test Case Name:
  * 005 - Functional test of the MainMenu (Scene 02_MainMenu)
* Component: 
  * Game Main Menu scene, 02_MainMenu
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * Travis Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * The user can make perform desired actions on the menu: Play, Quick Play, Controls, Settings, Quit and Credits
* Test Description/Purpose:
  * Perform detailed functional tests on Cyber Blitz game 02_MainMenu when accessed from a paused match/game
  * Main Menu test the button functionality and navigation of this scene
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has both a game controller and mouse attached.
  * Game started normally, user stated match, paused match and clicked the Main Menu button on the Pause panel.
#### Test Steps: 
#####  Main Menu (02_MainMenu) Main Menu and all buttons function
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Click 'Play' | Display transitions to the game setup scene (03_GameSetup) "Choose Yout Blitzer" panel | |			
| 2 | Click 'Quick Play' or press controller A | Go to the default scene (Cave Arena) and play the default match | |			
| 3 | Click 'Controls' or press controller A | Drops a 'Help' panel that explains the controls | |
| 4 | Click on 'Close' or press controller A | 'Help' panel raise from screen | |
| 5 | Click 'Settings' or press controller A | Drops a Settings panel that allows the user to change some settings | |
| 6 | Click on 'Close' or press controller A | 'Settings' panel raise from screen | |
| 7 | Click 'Credits' or press controller A | Drops a panel with game credits and copyrights | |	
| 8 | Click on 'Close' or press controller A | 'Settings' panel raise from screen | |
| 9 | Click 'Quit' or press controller A | Exits the application | |			
#### Overall Test Status:

### Test Case 6 - Functional test of the Game Setup scene (03_GameSetup) Player setup panel when loaded before game play - test two and four player modes and keyboard-mouse and game controllers
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID: 
  * 006
* Test Case Name:
  * Test Case 006# - Functional test of the Game Setup scene (03_GameSetup) Player setup panel when loaded before game play - test two and four player modes and keyboard-mouse and game controllers
* Component: 
  * Game Setup scene - 03_GameSetup
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * The functions of the game setup scene (03_GameSetup) and its two main panels
  * "Chooze Your Blitzer" to input player setup options of:
    * The number of players, 2 or 4
    * Who/What control of each player, User or Computer
    * The avatar of each player, Bat Bot, Cole Bot, Girls Bot or Panda Bot
    * The controller for each player (Computer or selected from detected controllers
    * Enforce one and only one controller per player rule
  * "Match Settings" to enter match options.
    * The arena to play in
    * The match time, one, two, three (default, or 5 minutes
    * The balls that will become available in a match, Neon, Bomb, Freeze, Asian, Homing
* Test Description/Purpose:
  * The game displays the "Choose Your Blitzer" panel from the 'Play' button on Main Menu
  * "Chooze Your Blitzer" to input player setup options of:
    * The number of players, 2 or 4 test number of players toggle button
    * Who/What control of each player, User or Computer Toggle button on top of avatar picture
    * The avatar of each player, Bat Bot, Cole Bot, Girls Bot or Panda Bot, click the picture to cycle and select
    * The controller for each player Computer or selected from detected controllers, select from available from dropdown button
    * Enforce one and only one controller per player rule, one controller controls 2 or more avatars
  * "Match Settings" to enter match options.
    * The arena to play in clicking slection button changes the arena as shwon by large arena image
    * The match time, one, two, three (default, or 5 minutes clicking side arrows cycles through these times
    * The balls that will become available in a match, Neon, Bomb, Freeze, Asian, Homing Neon selected by default, one or more ball types must get selected.

* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has both a game controller and mouse attached.
  * Game started normally, user selected play from the Main Menu.
#### Test Steps: 
##### Game Setup (03_GameSetup) - 'Choose Your Blitzer' Player selection buttons work correctly
| # | Description | Expected Result | Check (√) |
| - | ----------- | --------------- | --------- |
| 1 | Players shown on 'Choose Your Blitzer' panel at game setup entry | Display the default number of players with default avatars as a function of detected controllers | |			
| 2 | Players shown on 'Choose Your Blitzer' panel at after setup entry | Display the selected number of players with selected avatars and selected controllers | |	
| 3 | Use mouse to roll over buttons | Buttons show highlighted/selected | |
| 4 | Use left joystick or d-pad on cntroller to select buttons | Buttons show highlighted/selected | |
| 5 | Click on Player header or press controller A | Change weather the avatar get controlled by the user or the computer | |			
| 6 | Click on Players picture or press controller A | Change the player's avatar but not color. | |			
| 7 | Select drop down or press controller A | Change the controller used to control the avatar to selection | |			
| 8 | Click on 2 or 4 players or press controller A | Change between two and for players | |			
| 9 | Click on Main Menu or press controller A | Go back to the Main Menu | |			
| 10 | Click on Next or press controller A | Go to the Match Settings panel | |			
##### Game Setup (03_GameSetup) Match Settings buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Display on first entry to panel | Display the default arena, balls and match time. | |	
| 2 | Display subsequent panel entries | Display the selected arena, selected match time and selected balls | |	
| 3 | Use mouse to roll over buttons | Buttons show highlighted/selected | |
| 4 | Use left joystick or d-pad on cntroller to select buttons | Buttons show highlighted/selected | |
| 5 | Click on balls or press controller A | Allow the user to select or deselect the match balls | |			
| 6 | Click on time arrows or press controller A | Allow the user to increase or decrease the match time | |			
| 7 | Click on Arena or press controller A | Allow the user to select the arena to play | |			
| 8 | Click on Blitz or press controller A | Go play game in selected arena | |			
| 9 | Click on Back or press controller A | Go back to the player setup panel "Choose Your Blitzer" | |			
#### Overall Test Status:

### Test Case 7 - Functional test of the Game Setup scene (03_GameSetup) Player setup panel when loaded after game play has started - test two and four player modes and keyboard-mouse and game controllers
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID: 
  * 007
* Test Case Name:
  * Test Case 007# - Functional test of the Game Setup scene (03_GameSetup) Player setup panel when loaded after game play has started - test two and four player modes and keyboard-mouse and game controllers
* Component: 
  * Game Setup scene - 03_GameSetup
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * The functions of the game setup scene (03_GameSetup) and its two main panels
  * The scene will reset player and match settings to defaults on entry from game play
  * "Chooze Your Blitzer" to input player setup options of:
    * The number of players, 2 or 4
    * Who/What control of each player, User or Computer
    * The avatar of each player, Bat Bot, Cole Bot, Girls Bot or Panda Bot
    * The controller for each player (Computer or selected from detected controllers
    * Enforce one and only one controller per player rule
  * "Match Settings" to enter match options.
    * The arena to play in
    * The match time, one, two, three (default, or 5 minutes
    * The balls that will become available in a match, Neon, Bomb, Freeze, Asian, Homing
* Test Description/Purpose:
  * The game displays the "Choose Your Blitzer" panel from the 'Play' button on Main Menu
  * The scene will reset player and match settings to defaults on entry from game play
  * "Chooze Your Blitzer" to input player setup options of:
    * The number of players, 2 or 4 test number of players toggle button
    * Who/What control of each player, User or Computer Toggle button on top of avatar picture
    * The avatar of each player, Bat Bot, Cole Bot, Girls Bot or Panda Bot, click the picture to cycle and select
    * The controller for each player Computer or selected from detected controllers, select from available from dropdown button
    * Enforce one and only one controller per player rule, one controller controls 2 or more avatars
  * "Match Settings" to enter match options.
    * The arena to play in clicking slection button changes the arena as shwon by large arena image
    * The match time, one, two, three (default, or 5 minutes clicking side arrows cycles through these times
    * The balls that will become available in a match, Neon, Bomb, Freeze, Asian, Homing Neon selected by default, one or more ball types must get selected.

* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has both a game controller and mouse attached.
  * Game started normally, user changed default settings from the Game setup scenes then paused game and selected MainMenu and then selected Play.
#### Test Steps: 
##### Game Setup (03_GameSetup) - 'Choose Your Blitzer' Player selection buttons work correctly
| # | Description | Expected Result | Check (√) |
| - | ----------- | --------------- | --------- |
| 1 | Players shown on 'Choose Your Blitzer' panel at game setup entry | Display the default number of players with default avatars as a function of detected controllers | |			
| 2 | Players shown on 'Choose Your Blitzer' panel at after setup entry | Display the selected number of players with selected avatars and selected controllers | |	
| 3 | Use mouse to roll over buttons | Buttons show highlighted/selected | |
| 4 | Use left joystick or d-pad on cntroller to select buttons | Buttons show highlighted/selected | |
| 5 | Click on Player header or press controller A | Change weather the avatar get controlled by the user or the computer | |			
| 6 | Click on Players picture or press controller A | Change the player's avatar but not color. | |			
| 7 | Select drop down or press controller A | Change the controller used to control the avatar to selection | |			
| 8 | Click on 2 or 4 players or press controller A | Change between two and for players | |			
| 9 | Click on Main Menu or press controller A | Go back to the Main Menu | |			
| 10 | Click on Next or press controller A | Go to the Match Settings panel | |			
##### Game Setup (03_GameSetup) Match Settings buttons work correctly
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Display on first entry to panel | Display the default arena, balls and match time. | |	
| 2 | Display subsequent panel entries | Display the selected arena, selected match time and selected balls | |	
| 3 | Use mouse to roll over buttons | Buttons show highlighted/selected | |
| 4 | Use left joystick or d-pad on cntroller to select buttons | Buttons show highlighted/selected | |
| 5 | Click on balls or press controller A | Allow the user to select or deselect the match balls | |			
| 6 | Click on time arrows or press controller A | Allow the user to increase or decrease the match time | |			
| 7 | Click on Arena or press controller A | Allow the user to select the arena to play | |			
| 8 | Click on Blitz or press controller A | Go play game in selected arena | |			
| 9 | Click on Back or press controller A | Go back to the player setup panel "Choose Your Blitzer" | |			
#### Overall Test Status:

# Test Case 8 - Functions test of the game in the SA Neodome Arena (scene 04_NeonArena) - Camera, Character, Controll, animations and sound for keyboard/mouse user controlled characters, two and four player modes.
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 008
* Test Case Name:
  * Test Case 008 - Functions test of the game in the SA Neodome Arena (scene 04_NeonArena) - Camera, Character, Controll, animations and sound for keyboard/mouse user controlled characters, two and four player modes.
* Component: 
  * Game Scene SA Neodome - 04_NeonArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with keyboard-mouse
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Use of keyboard mouse for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with keyboard-mouse - AWSD and Arrow keys for movement, E - dodge, Left Mouse - 'charge' throw, Right Mouse - pickup catch, mouse movement for aim (target tracks hidden cursor)
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has a mouse attached.
  * Game started normally, user has one avatar controlled by key-board mouse, and none to three controlled by controllers and noe to three controlled by the computer.
  * User has selected SA Neodome Arena then clicked the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Click Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Press A or left arrow | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Press W or up arrow | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Press S or down arrow | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Press D or right arrow | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press E | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Left mouse button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Left mouse button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Left mouse button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press Right mouse button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press Right mouse button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |
#### Overall Test Status:

# Test Case 9 - Functions test of the game in the Lumos Arena (scene 05_CaveArena) - Camera, Character, Controll, animations and sound for both user keyboard/mouse controlled characters characters, two and four player modes.
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 009
* Test Case Name:
  * Test Case 009 - Functions test of the game in the Lumos Arena (scene 05_CaveArena) - Camera, Character, Controll, animations and sound for keyboard/mouse controlled characters, two and four player modes.
* Component: 
  * Game Scene Lumos Arena - 05_CaveArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with keyboard-mouse
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Use of keyboard mouse for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with keyboard-mouse - AWSD and Arrow keys for movement, E - dodge, Left Mouse - 'charge' throw, Right Mouse - pickup catch, mouse movement for aim (target tracks hidden cursor)
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has a mouse attached.
  * Game started normally, user has one avatar controlled by key-board mouse, and none to three avatars controlled by controllers and one to three avatars controlled by the computer.
  * User has selected Lumos Arena then clicked the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Click Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Press A or left arrow | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Press W or up arrow | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Press S or down arrow | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Press D or right arrow | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press E | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Left mouse button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Left mouse button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Left mouse button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press Right mouse button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press Right mouse button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |
#### Overall Test Status:

# Test Case 10 - functions test of the game in the Song Shu Street Arena (scene 06_AsianArena) - Camera, Character, Controll, animations and sound for both user keyboard/mouse controlled characters, two and four player modes.
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 010
* Test Case Name:
  * Test Case 010 - Functions test of the game in the Song Shu Street Arena (scene 06_AsianArena) - Camera, Character, Controll, animations and sound for both user keyboard/mouse controlled characters, two and four player modes.
* Component: 
  * Game Scene Song Shu Street Arena - 06_AsianArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with keyboard-mouse
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Use of keyboard mouse for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with keyboard-mouse - AWSD and Arrow keys for movement, E - dodge, Left Mouse - 'charge' throw, Right Mouse - pickup catch, mouse movement for aim (target tracks hidden cursor)
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has a mouse attached.
  * Game started normally, user has one avatar controlled by key-board mouse, and none to three avatars controlled by controllers and one to three avatars controlled by the computer.
  * User has selected Song Shu Street Arena then clicked the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Click Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Press A or left arrow | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Press W or up arrow | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Press S or down arrow | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Press D or right arrow | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press E | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Left mouse button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Left mouse button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Left mouse button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press Right mouse button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press Right mouse button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |
#### Overall Test Status:

### Test Case 11 - Functions test of the game in the SA Neodome Arena (scene 04_NeonArena) - Camera, Character, Controll and animations and sound for game controller user controlled characters, two and four player modes..
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 011
* Test Case Name:
  * Test Case 011 - Functions test of the game in the SA Neodome Arena (scene 04_NeonArena) - Camera, Character, Controll, animations and sound for game controller user controlled characters, two and four player modes.
* Component: 
  * Game Scene SA Neodome - 04_NeonArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with generic x box controller
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Use of generic x box controller for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with 'generic' X Box controller - Left joy stick D-Pad for movement, X to dodge, A pickup catch, Right bumper - 'charge' throw.
  * Avatar controlled by by computer
  * Avatar can pickup ball
  * Avatar cannot 'steal' ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has a game controller attached.
  * Game started normally, user has one to four controlled by controllers, one to three avatars controlled by the computer and 0 to one avatar controlled by the keyboard/mouse (tests for controller only).
  * User has selected SA Neodome Arena then selected (A button) the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Select (A) Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Left Joy stick Left or Left on D-pad | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Left Joy stick Up or Up on D-pad | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Left Joy stick Down or Down on D-pad | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Left Joy stick Right or Right on D-pad | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press X button | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Right Bumper button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Right Bumper button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Right Bumper button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press A button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press A button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |
#### Overall Test Status:

### Test Case 12 - functions test of the game in the Lumos Arena (scene 05_CaveArena) - Camera, Character, Controll, animations and sound for both user game controller controlled characters, two and four player modes.
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 012
* Test Case Name:
  * Test Case 012 - Functions test of the game in the Lumos Arena (scene 05_CaveArena) - Camera, Character, Controll, animations and sound for both user game controller controlled characters, two and four player modes.
* Component: 
  * Game Scene Lumos Arena - 05_CaveArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with generic x box controller
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Must have keyboard mouse for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with generic x box controller - Left joy stick D-Pad for movement, X to dodge, A pickup catch, Right bumper - 'charge' throw.
  * Avatar controlled by by computer
  * Avatar can pickup ball
  * Avatar cannot 'steal' ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has a game controller attached.
  * Game started normally, user has one to four controlled by controllers, one to three controlled by the computer and one or none keyboard/mouse controlled avatars.
  * User has selected Lumos Arena then clicked the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Select (A) Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Left Joy stick Left or Left on D-pad | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Left Joy stick Up or Up on D-pad | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Left Joy stick Down or Down on D-pad | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Left Joy stick Right or Right on D-pad | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press X button | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Right Bumper button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Right Bumper button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Right Bumper button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press A button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press A button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |

#### Overall Test Status:

### Test Case 13 - Functions test of the game in the Asian Arena (scene 06_AsianArena) - Camera, Character, Controll, animations and sound for both user game controller controlled characters, two and four player modes.
##### Team_E(xcellence) G. Broughton, B. Heath, T. Womack
##### 10/24/2017
##### Ver 0.8
* Test Case ID:
  * 013
* Test Case Name:
  * Test Case 013 - Functions test of the game in the Song Shu Street Arena (scene 06_AsianArena) - Camera, Character, Controll, animations and sound for both user game controller controlled characters, two and four player modes.
* Component: 
  * Game Scene Song Shu Street Arena - 06_AsianArena
* Test Case Designer:
  * Travis Womack
* Creation Date:
  * 10/17/2017
* Modified By:
  * B. Heath, T. Womack
* Modified Date:
  * 10/24/2017
* Requirements Covered:
  * Display of starting animation
  * Display of 2 player UI in 2 player mode
  * Display of 4 player UI in 4 player mode
  * Avatar control by user with generic x box controller
  * Avatar can pickup ball
  * Avatar can throw ball
  * Avatar can catch ball
  * Avatar 'died' when hit
  * Covers Neon ball interactions only
  * Use of generic x box controller for one controller
* Test Description/Purpose:
  * Display of starting animation after loading scene
  * Display of 2 player UI in 2 player mode after start animation completes
  * Display of 4 player UI in 4 player mode after start animation completes
  * Avatar control by user with generic x box controller - Left joy stick D-Pad for movement, X to dodge, A pickup catch, Right bumper - 'charge' throw.
  * Avatar controlled by by computer
  * Avatar can pickup ball
  * Avatar cannot 'steal' ball
  * Avatar can throw ball
  * Avatar can only throw ball in attack area
  * Avatar has Orange X at base if Unable to attack
  * Avatar can catch ball
  * Avatar 'dies' when hit
  * Avatar has immunity after 'resurrection'
* Pre-Test Conditions:
  * Current build of the game will run on Windows 7 and 10 in a standalone environment.
  * The PC has both a game controller and mouse attached.
  * Game started normally, user has one or none avatar controlled by key-board mouse, one to four controlled by controllers and one to three controlled by the computer.
  * User has selected Song Shu Street Arena then selected (A button) the 'Blitz>>>' button
#### Test Steps: 
| # | Description | Expected Result | Check (√) |
| --- | --- | --- | --- |
| 1 | Select (A) Blitz (Game Setup) or Quick Play (MainMenu) | Display of starting animation after loading scene with music | |			
| 2 | End of start animation | Display of 2 player UI in 2 player mode after start animation completes | |			
| 3 | End of start animation | Display of 4 player UI in 4 player mode after start animation completes | |			
| 4 | Left Joy stick Left or Left on D-pad | Avatar move left while pressed or hits edge or center court with sound FX | |			
| 5 | Left Joy stick Up or Up on D-pad | Avatar move up while pressed or hits edge with sound FX | |			
| 6 | Left Joy stick Down or Down on D-pad | Avatar move down while pressed or hits edge with sound FX | |			
| 7 | Left Joy stick Right or Right on D-pad | Avatar move right while pressed or hits edge or center court with sound FX | |			
| 8 | Press X button | Plays dodge animation and moves 2 units infacing direction with sound FX | |			
| 9 | Press Right Bumper button | Avatar with ball starts charging holds charge as lon as button pressed with sound FX | |	
| 10 | Release Right Bumper button | Plays throw animation and propells ball in aimed direction with sound FX | |
| 11 | Release Right Bumper button with orange X | Ball does not get thrown - can only throw behind attack line with sound FX | |
| 12 | Press A button | Avatar can pickup ball if close enough and not held by another avatar with sound FX | |			
| 13 | Press A button | Avatar without ball can catch ball if close enough with no hit with sound FX | |			
| 14 | Move mouse | Aiming target moves and aim arrow follows target | |			
| 15 | Avatar hit by ball thrown by enemy | Avatar 'dies' (disappears) when hit | |			
| 16 | Avatar placed at start point | Avatar has immunity after 'resurrection' does not die if hit within 2 seconds after placement | |
#### Overall Test Status:

### Acceptance Criteria (Estimated number of defect or internal test acceptance criteria)
These tests will have an overall acceptance criteria of 70% for the Alpha build(s) and 90% for the Beta Builds
### References (List any reference documents)
Game Design document in the Google Docs folder: https://drive.google.com/drive/folders/0B3sX0N3yT3LucVBWTEFzbGQwbUE
Technical Design Document in the Google Docs folder: https://drive.google.com/drive/folders/0B3sX0N3yT3LucVBWTEFzbGQwbUE
## Plan
Currently we plan on the following testing schedule:

Develop Schedule     Start: October 1, 2017 - Comlete: October 16, 2017    G. Broughton, B. Heath, T. Womackd

Game Selection       Start: October 11, 2017 - Comlete: October 16, 2017   G. Broughton, B. Heath, T. Womack

Create Test Plan     Start: October 11, 2017 - (first draft October 31) Comlete: November 7, 2017  G. Broughton, B. Heath, T. Womack

Create Test Cases    Start: October 11, 2017 - Complete: October 30, 2017   G. Broughton, B. Heath, T. Womack

Execute Test Cases   Start: November 6, 2017 - Complete: November 13, 2017  G. Broughton, B. Heath, T. Womack

Create Test Report   Start: November 15, 2017 - Complete: November 22, 2017 G. Broughton, B. Heath, T. Womack

Send Status Report 1 Start: October 1, 2017 - Complete: October 16, 2017    G. Broughton, B. Heath, T. Womack

Send Status Report 2 Start: November 14, 2017 - Complete: November 21, 2017 G. Broughton, B. Heath, T. Womack
## Specifications will get covered in the individual test case documents, results and and evaluations follow.
### [Test Case 001](Team_E_Test_Case_01.md)
#### Overall Test Status:
Main Menu Cyber Blitz appears over all drop downs - minor bug

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 06, Nov. 2017 | T. Womack | Pass with minor bug (see above) |			

### [Test Case 002](Team_E_Test_Case_02.md)
#### Overall Test Status:
Passed 
#### Bugs: CyberBlitz logo on main menu stays on top of drop down panels - minor bug

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 06, Nov. 2017 | T. Womack | Passed with minor bug see above |			

### [Test Case 003](Team_E_Test_Case_03.md)
#### Overall Test Status:
Passed - no bugs found

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 07-Nov. 2017 | T. Womack | Passed |			

### [Test Case 004](Team_E_Test_Case_04.md)
#### Overall Test Status:
Passed

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 07, Nov. 2017 | T. Womack | Passed |			

### [Test Case 005](Team_E_Test_Case_05.md)
#### Overall Test Status:
Passed tests as stated.
Failed new requirement to reset to defaults when entering from game play - bug report submitted

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 07, Nov. 2017 | T. Womack | Passed tests as stated - failed new requirement |			

### [Test Case 006](Team_E_Test_Case_06.md)
#### Overall Test Status:
#### Bugs: On quick play selection, Crystal stage default, Maya and Max. Maya picks up ball, and controls freeze. Maya does not charge nor throw the ball. Maya respawns with ball and still cannot throw. Maya drops the ball, with a ball remaining on her head. Orange X does not appear during control freeze. This is caused when Maya catches the ball on the line between the non-throw and throw area. To repeat, place Maya on the line between the throw and non-throw area. The X may or may not appear. Catch the ball from the computer, and eventually Maya's controls with freeeze. If the dodge is pressed while this error is occurring, the ball will move 10-20 units away. Maya will still be unable to throw, and when she dodges the ball rotates around with her. Error also occurs if player picks up more than one ball. Maya will throw the extra ball on her head, however the other ball will remain on her head, and charge does not appear. Dodge error implimented creates the flying ball error once more, causing it to follow player for a short period. wherever the player looks the ball follows. Up to twq balls can float around the player. They may or may not respawn. AI will follow the floating balls. Dodging approx. 2-4 times will cause the balls to fly. AI can pick-up flying ball if it is within reach. Maya's Catch state becomes permanant during this error and cannot be killed by AI. Repeatable in ALL stages. Repeatable in ALL players. Players remain in idle animation, hands stay close to the body.

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 11/10/17 | B. Heath | Criteria is met for test, Bugs Discovered need to be addressed |			
| 2 | 11/10/17 | B. Heath | Catch Bug Dicovered in Quick Play |			
| 3 | 11/10/17 | B. Heath | Dodge Error, Ball follows player |			
| 4 | 11/10/17 | B. Heath | Multiple Ball Pick-up Freezes controls and creates a floating ball |
| 5 | 11/10/17 | B. Heath | Floating ball error can be up to two balls. balls may or may not respawn |						
| 6 | 11/10/17 | B. Heath | Unity Bat bot gets pushed by ball, whenever it is picked up |	
| 7 | 11/10/17 | B. Heath | AI can steal ball from player as long as you are in the no-throw zone |	
| 8 | 11/10/17 | B. Heath | Credits Scene does not close out when the close button is pressed |	

### [Test Case 007](Team_E_Test_Case_07.md)
#### Overall Test Status:
#### Bugs: Selecting Random stage, switches between neon and crystal only. Asia stage has been left out. On win for Quick play, "NOBODY WINS" text is displayed. Score does not matter, and text is continuously displayed. On player selection screen, in two player mode, switching the computer to player, causes both characters to be controlled by the player. characters can throw, grab and die, and they both follow player one's mouse. Player can accidently pick up a secondary ball, if it spawn while they pick up another. This requires good timing but is repeatable.Entering match settings menu for the first time, the cyrstal stage shows on the preview screen. On Pressing blitz, the neon stage is selected. This is a confusing factor. Perhaps add a blank option(or default to random) for on enter to prevent confusion. 

#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 11/10/17 | B. Heath | Criteria is met for test, Bugs Discovered need to be addressed |
| 2 | 11/10/17 | B. Heath | Asia Stage not Included in Random Stage Selection |	
| 3 | 11/10/17 | B. Heath | Nobody wins is displayed on win by either team |
| 4 | 11/10/17 | B. Heath | Single player can controll all characters by switching to user control |
| 5 | 11/10/17 | B. Heath | Multiple Ball-Pick up while picking up another ball |			
| 6 | 11/10/17 | B. Heath | On match settings, default stage is lumos arena, and when played, default is neon |			

### [Test Case 008](Team_E_Test_Case_08.md)
#### Overall Test Status:
#### Bugs: Settings Panel in pause menu is a dead end. Button Highlights and remains highlighted.
#### Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 11/10/17 | B. Heath | Pause menu settings remains selected and goes nowhere |

### [Test Case 009](Team_E_Test_Case_09.md)
#### Overall Test Status:
Passed with one bug - created HnP bug report #397, settings Panels does not drop when selected from Pause panel

#### Bugs
1 bug found Settings Panels does not drop when selected from Pause panel, HnP bug report #397

## Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 12 Nov. 2017 | T. Womack | 1 bug found Settings Panels does not drop when selected from Pause panel |			

### [Test Case 010](Team_E_Test_Case_10.md)

## Overall Test Status:
Passed - visuals incomplete for level/arena/scene

#### Bugs:
Settings panel not dropped when selecte from pause panel.

## Run History:
| # |	Run Date |	Run By |	Results |
| --- | --- | --- | --- |
| 1 | 11/10/17 | B. Heath | Criteria is met for test, Bugs Discovered need to be addressed |

### [Test Case 011](Team_E_Test_Case_11.md)

### [Test Case 012](Team_E_Test_Case_12.md)

### [Test Case 013](Team_E_Test_Case_13.md)
