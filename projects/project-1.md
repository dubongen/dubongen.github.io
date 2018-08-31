---
layout: project
type: project
image: images/olympic1.jpg
title: Olympic Race Game
permalink: projects/olympicrace
# All dates must be YYYY-MM-DD format!
date: 2016-10-24
labels:
  - Java
  - Eclipse
summary: In ICS 111 we've created a racing game that let's you race against the CPU.
---

<div class="ui small rounded images">
  <img class="ui image" src="../images/Screen Shot 2018-08-30 at 4.35.07 PM.png">
</div>

This project was given to me and my ICS 111 class by Jason Leigh. It was a way to introduce the class to game development and inspire some of new programers to persue coding and encourage them to keep trying and perservere. The requirements of the program is to have three racers and one of those racers you are controlling by pressing the keys 'W' and 'S'in a sequential order. While you are controlling your character's movement, the CPU is generating a random value to either increase their movement or to decrease it. This forces you to continuously pressing 'W' and 'S' to the point where you just might end up breaking your keyboard just so that you can win.

With this project I've ran into some difficulties with meeting the requirements, these included syntax errors, my code not loading my images for the task and missing files in my eclipse. All of this brought mentally straining hours and frustration, this was mostly due to the fact that it was my first time programming on Eclipse and having minimal knowledge on this editing/programming software. What solved this problem and helped me complete this project was my TA, and he took a file from my Eclipse admin folder and he got my work to finish. This actually made me realize that sometimes it's not your coding that has the problem it could be the files that are in your project.

With this project, it gave me an idea of how it's like to develop a game even if it's something small like this project.

Sample of Code

    while (isracing){

      Zoom.translateBy (rand.nextInt(4),0); //random integer multiplied by x value of racer's coordinates			
			ReverseFlash.translateBy (rand.nextInt(4),0); //random integer multiplied by x value of racer's coordinates
			
			EZ.refreshScreen(); //When screen refresh reset random integers
	
      Flash.translateTo(flashX,140);//translate the coordinates
			
			if (EZInteraction.wasKeyPressed(currkey)==true) { //set key interaction
				tem=lastkey;//temporary is the last key pressed
				lastkey=currkey;//the last key = the current key
				currkey=tem;//temporary is the current key pressed
				Flash.translateBy (5+rand.nextInt(8),0);	// when keys is pressed add 5 and a random int to flashX
			}	



