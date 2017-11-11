2017_03_11 Design Notes

Elven Scholar
	Elf goes around, talks to peeps in cities, they give info and ask
		"Please, there are things that I am meant to remember, can you please help me to?" 
		-->input question
		"What is the answer, on Scholar?"
		-->input answer

 	Can import questions from CSV

 	Info peeps guide the story line, ie
 		"There's a monster in the cave NE of here, bla bla bla"


 	classes
 		Elf
 		Human
 		Orc
 		Halfling
 		Dwarf
 		Goblin

 		Or, to keep in line with the new story, our hero is only an Elf, so as to complicate things less
 			No novice state
 				XP is not a stat, instead, correct questions improve demon at the level of casting, incorrect answers diminish efficacy of demon skill
 					each demon imparts 3 skills, 1 attack, 1 defense, 1 other?

 	Re Questions
 		these are kept in a JSON file
 			Question (can have images), Answer, #correct answers, #missed questions
 				Overall Question Queue... every time you put in a new question, it goes to the end of the queue
 				Active Question Queue... these are the questions that can be asked from

 		Game depends on size of queue so player has to grind to open new levels.  if there aren't enough questions, can't unlock new levels or new regions - this motivates the player to add more questions

 		Chris - "Does a level 3 enemy require a level 3 question or can it be a level 1 question?"
 			questions are just active or inactive depending on the general success ratio of the question, question will appear more or less often

 	Originally was thinking of a simple static map or procedural map generation

 	Attacks
 		attack spells have an inherent max damage as a multiplier of various characteristics

 	GUI
 		need an add question button to put things on the end of the queue

 	Levels/World
 		Story
 			world is massive and the mentor/fox daemon in a box that the scholar has been learning from his own life, tells the scholar to go to the island from where he's from. the island is a giant who strayed from their land and fell into the ocean and died.  Each region of the land is a region of the giants body, with names and cities corresponding to parts of the anatomy.
 			evil descending on the land that will spread to the rest of the earth
 				find out later that it's the mnemophages who feed off of memories, in league with a necromancer who will raise the dead demon as a vessel to destroy the world
 				mnemophages shoot electricity to eat memories
 					1 mnemophage boss every 2 levels, with lesser bosses or puzzles on the others

 		level 1 is green, verdant--> level 17 will be brimstone
 			1 - left foot
 				foxes

 			2 - right foot
 				raccoon

 			3 - lower left leg
 				deer

 			4 - lower right leg
 				elk

 			5 - upper left leg
 			6 - upper right leg
 			7 - left hand
 			8 - right hand
 			9 - left forearm
 			10 - right forearm
 			11 - left upper arm
 			12 - right upper arm
 			13 - crotch
 			14 - abdomen
 			15 - chest
 			16 - neck
 			17 - head
 				spiders

 		Level 1, the left foot, is a tutorial and the land from where the fox daemon is from.
 			this daemon allows practice
 				don't get gold or xp or hp
 				does affect question percentage

 		levels 1-6, answer 1 question per skill
 		levels 7-12, answer 2 questions
 		levels 13-17, answer 3 questions

 	Each demon has 3 skills/spells imparted
 		demon 1 gives basic attack, basic defense, basic escape
 			answer 1 question
 		crotch demon 13 gives recover HP, etc

 	Items
 		Life potions as drops
