# CSE 571 Team Project Guide

There are two folders for this team project. Please run them separately. 

### Files that we have

* multiagent folder
* reinforcement folder
* README file
* Final Report

### Informations

a.  Team name: Pacman the Ghostrider

b.  Names of the team members: Amit Sharma, Vishwarajsinh Sodha, Wei Xin, Sajjan Kumar 

c.  Topic chosen : Topic 3 Games & Theory of Mind

d.  contributions of each team member: 

   	Expectimax and Minimax Skeleton: Amit, Sajjan
	Probability algorithm implementation:	Wei, Vishwaraj
	Evaluation function:	Wei, Vishwaraj, Sajjan, Amit
	Analysis and reasoning:	Wei, Vishwaraj
	Testing and Review:	Amit, Sajjan, Wei, Vishwaraj

e.  instructions to run your code from scratch:

### Setup and Initialization

* Operating System used windows.
* Install `python 2.7` and ensure it is in path
* Install matplotlib using -> 
  `python2 -m pip install matplotlib` 
  (If matplot already installed and you are facing some issues then uninstall using pip uninstall matplotlib , followed by the above        command to install matplotlib. )
* Clone the repository
* Go to `multiagent` directory
* Inside the directory run command `python pacman.py -p MinimaxAgent -l minimaxClassic -k 2 -n 5 -q`  
* If the above command runs fine, the setup is correct

### For Multiagent: (You can also go to the Multiagent folder and follow the README file)
	
NOTE - (Use python2 or python whichever runs python 2 for your environment)
The setup is very similar to Project 2 ... Only additional thing is we have used matplotlib

Commands that can be used for running :-

REMINDER - (Use python2 or python whichever runs python 2 for your environment)

(In below commands I have used python2 ... If that doesn't work then try python ... If that also doesn't work then use py -2)


------------   minimaxClassic Layout with 2 ghosts ----------------------------

python pacman.py -p MinimaxAgent -l minimaxClassic -k 2 -n 5 -q

python2 pacman.py -p ExpectimaxAgent -l minimaxClassic -k 2 -n 5 -q

python2 pacman.py -p MinimaxAgent -l minimaxClassic -k 2 -n 5

python2 pacman.py -p ExpectimaxAgent -l minimaxClassic -k 2 -n 5


---------------------------------------------------------------------------------

------------   trappedClassic Layout with 1 ghost ----------------------------

python2 pacman.py -p MinimaxAgent -l trappedClassic -k 1 -n 5 -q
 
python2 pacman.py -p ExpectimaxAgent -l trappedClassic -k 1 -n 5 -q

python2 pacman.py -p MinimaxAgent -l trappedClassic -k 1 -n 5
 
python2 pacman.py -p ExpectimaxAgent -l trappedClassic -k 1 -n 5

-------------------------------------------------------------------------------

STEP 2:
After you execute any of the above command.
Kindly enter the Reasoning Level Depth upto which you want to explore. 

For example - You give 6
Then our agent will run 'n' games for reasoning level 1, level 2, ..till... level 6
Then finally our ANALYZER agent will display ANALYSIS of pacman performance through each of these levels and categorize 1 to 6 levels in three different categories as UNDERTHINKING, OPTIMAL and OVERTHINKING.


NOTES:-

1) TrappedClassic runs very fast, so allowing agent to explore more reasoning levels for each game - (1 to 8 levels)

2) MinimaxClassic runs very slow, so allowing agent to explore less reasoning levels - (1 to 6 levels) ... level 6 might take a little more time - so if you want to avoid that you can give 5 as max reasoning level

#### Final analysis:-

The analysis is displayed towrds the end of execution of all levels. 
It shows the CLASSIFICATION of levels into :
UNDERTHINKING levels
OPTIMAL level
OVERTHINKING levels


### For Reinforcement Learning: (You can also go to the reinforcement folder and follow the README file)

Same set up as Multiagent 

Commands that can be used for running :-

(Use python2 for python2 environment ... otherwise python should be fine)

python pacman.py -p PacmanQAgent -x 2000 -n 4000 -l smallGrid -q -f --fixRandomSeed

Note that at line 611 of game.py, a user can modify the agentIndex = self.startingIndex into agentIndex = 1 to test the ghost level.
