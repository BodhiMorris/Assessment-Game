# __rainy Software Design Proposal__  


## __Identifying the Need__  


__Need__  
I want to create a cosy game with simple mechanics and a motif of water. Inspiration from games like rain world, Ori and the will of the wisps, TOTK, hollow night and my friendly neighbour Totoro




__Problem Statement__  
A Lot of people try to make ambitious games with complicated finicky mechanics that end up feeling unpolished and unrefined leading to the game being unpleasant to play. I plan to make a simple 2D platformer where the focus is on the atmosphere rather than game mechanics and story. I want the game to feel very nice and polished.




__Skill Development__  
Being a simple game in terms of mechanics I could probably use the tutorial that you provided us or ask my brother who is into gamedev and would know good resources that I could watch on YouTube. I would have to develop skills in my sound design to achieve the wanted feel of the game, and I would have to develop skills in game/level design.




__Brainstorm__  
cosy game  
focus on sound design  
wandering through areas  




emerge from water  
rain  
leaf umbrella  
dino  
lizard  
cat in bakery*  




ends in field of flowers just after rain stops  Rainy
enjoyment of the silence once the game ends  
natural setting, rain forest, cave, field,  


Lizard like character making its way through the sewers and underground where it finally makes it to the surface where it is nice and rainy




|Game|Positive|Minus|Implication|  
|---|---|---|---|
|![alt text](image.png)|While playing this game I really enjoyed the movement and art|This game copied hollow knights mechanics and general gameplay loop|I would like to make the movement feel as smooth as this game without copying the other mechanics and gameplay loop from hollow knight or another game|
|![alt text](image-1.png)|I really enjoyed the aesthetic of the game and how you are not important in the game, your a pray at the bottom of the food chain trying to survive|I didn't really enjoy the game as it felt like I was missing knowledge of where to go, especially since you were on a clock against the rain|I would like to emulate the feeling you get from playing rain world without the pressure of the clock|
|![alt text](image-2.png)|I loved how the music reflected the world you are in and elevated the intended experience|The game doesn't give the feeling that I want my game to give|I would like to create an atmosphere and melodic accompaniment that elevates what I want my game to feel like.|




## __Requirements Outline__  




__Inputs:__ The only required inputs would be directional from the player  
__Proccessing:__ The game will check the players collision and position and if a step occurred  
__Outputs:__ The game will show the scene and player model to the player as well as the environmental, reactionary and maybe melodic sound  
__Transmision:__ This will be a single player, offline game  
__Storage:__ I will store the players levels completed and what level you are currently on locally  




### __Functional Requirements__  




__User Interaction__  
The user will use the directional keys on their keyboard (WASD + spacebar or arrows) and the mouse or a controller to move the character with two degrees of movement. The character will be able to move left and right and jump. The user will use their mouse to navigate menus in the game




__Core Gameplay or Simulation Mechanics__  
The only gameplay mechanics will be movement based, I will add normal 2d platformer movement like moving, jumping and wall jumps




__Level Progresion__  
I am going to have the levels be small and enclosed and transition in a way similar to hollow knight where the two adjacent levels are loaded so as to give a more seamless experience, there will be a trigger at the end of each level to track player level progress and which ones are completed.




__Saving and Loading Data__  
I will save a document that would contain information like which levels are completed and player controls.




### __Non-Functional Requirements__  




__Performance Requirements__  
I will aim for a stable framerate of at least 30fps, have the inputs feel instant with minimal delay and load the levels quickly or in a way that doesn't seem to take that long to the user, with a transition screen or something




__Usability Requirements__  
The game will include a simple at the start of the game to teach the user about the mechanics.




__Scalability__  
The game should be able to have extra levels added in future and still maintain my performance requirements.




### __Considerations of Social and Ethical Issues__  




__Equity__ is recognizing that people do not have the same requirements and giving people the support that they need.  
__Accessability__ is ensuring that everyone can use a product, no matter how they find it  




__Accessibility__  
I will take measures to make my game as accessible as possible. My game will have no words and writing, you will be able to use keyboard and mouse or a controller and there will be the ability to change the players controls making the game very accessible




__Privacy and Data Protection__  
My game will collect no personal data. The only things that my game would store would be required for the game to run properly such as the levels that have been completed, and game controls.




__Fairness and Representation__  
My game's character will either be a dinosaur or lizard and be in no way linked to racial stereotypes and my game areas will not be linked to any real world places/have people in them.




__Mental and Emotional Wellbeing__  
The idea of my game is to be a relaxing platformer which lets you enjoy the time you are spending. This will promote a healthy mindset and I will incorporate elements that make me happy like rain.




__Cultural Sensitivites__  
My game wont have any offensive content and will have little to no symbols as it is focused on the feeling of the area rather than what is actually in it.


## __Flowcharts__


*Attached in the flowcharts file


## __Pseudocode__


BEGIN Movement  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;INPUT userInput  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IF 'A' pressed THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Move player left  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ELSE IF 'D' pressed THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Move player right  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ELSE IF 'Spacebar' or 'W' pressed THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IF player touching ground THEN  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Move player jump  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;ELSE IF player on wall  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;More player walljump  
 
END Movement


-----------------------------------------------------------------------------------------------------------------------------------------------
   


BEGIN Level_Load  


&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;WHILE Game_Running == True  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Load PlayerLevel(n), PlayerLevel(n+1), PlayerLevel(n-1)  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;IF Menu_Selecet(Quit) == True  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Game_Running == False  


END Level_Load


-----------------------------------------------------------------------------------------------------------------------------------------------
   
BEGIN Progress_Save    
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;If Level(n), complete == TRUE  
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Print (n) to text document  


END Progress_Save


## __Story Boards__


![Whole game storyboard is attached](<Assesment game main story board.png>)  
the scene storyboards were handed in physically due to not being able to scan them properly


## __Gantt Chart__
I couldn't save the sheet as a pdf so here is a link so you can still view it  
https://docs.google.com/spreadsheets/d/1rjJ4KwI1wuyGXs3Cq1gmBSHrShUdK7UU8A34MAMzJM0/edit?usp=sharing

## Epic Music

https://www.youtube.com/watch?v=bBQA7yy7EBU&t=1150s  
https://www.youtube.com/watch?v=hvuojhm02Yk&t=1010s