# A-Path-Finder---AI-mini-project
Title: To find the shortest path between the source and the destination with walls in between.

Steps:
A* Algorithm
1. Put the start node s on OPEN.
2. If OPEN is empty, exit with failure
3. Remove from OPEN and place on CLOSED a node n having minimum f.
4. If n is a goal node exit successfully with a solution path obtained by tracing back the
pointers from n to s.
5. Otherwise, expand n generating its children and directing pointers from each child node to
n.
   5.1 For every child node n’ do
   5.2 evaluate h(n’) and compute f(n’) = g(n’) +h(n’) = g(n)+c(n,n’)+h(n)
   5.3 If n’ is already on OPEN or CLOSED compare its new f with the
        old f and attach the lowest f to n’.
   5.4 put n’ with its f value in the right order in OPEN
6. Go to step 2.




After properly installing Python 2.6 and PyGame, to execute this demo:

$ python path.py

How to use it:

Cell Placement:

Place/Remove Start square       - CTRL + LEFT_CLICK
Place/Remove Goal square        - CTRL + RIGHT_CLICK
Place/Remove a Wall square      - SHIFT + LEFT_CLICK
		Note: 	You can hold this down and move the cursor to place several 	
				walls at a time
				
Reset Board:

Clear the entire board          - ESCAPE
Soft clear board                - BACKSPACE
		Note:	Leaves Start, Goal and Wall squares
		
Find Optimal Path:

Verbose Mode                    - ENTER
Instant	                        - RIGHT_ARROW
Step Through Path               - N

Change Heuristics:

"Straight Line Distance"        - SHIFT + 1
"Manhattan Distance"            - SHIFT + 2
"Zero" (Nothing Known)          - SHIFT + 3
