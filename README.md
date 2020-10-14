# Assignment 2:  HOMER

In this assignment, you will implement the HOMER interaction technique described in section 7.9.1 of the textbook. You may implement this using any of the 3 environments from Assignment 1 (Babylon.js, Playcanvas Editor, or Playcanvas Engine).  This template is empty (except for a .gitignore file and this README.md);  you should fill in the project with something similar to 1(a), 1(b), or 1(c) and follow the corresponding instructions for submission.

The goal of the assignment is to have you gain experience with implementing a non-trivial interaction technique (and, incidentally, setting up the project based on a previous one.)

You can see HOMER in action in this old [YouTube Video](https://www.youtube.com/watch?v=V6Fo3iza5cY) by Doug Bowman that illustrates how it works in practice. (Ignore the "camera motion" part and just pay attention to the object motion part.)

In the book, they mention that the algorithm relies on some "scaling constants" but does not provide details.  [Here are some slides](resources/interaction_part1.pdf) from one of Doug's old lectures that explain those constants.

## Due: Monday October 26th, 11:59pm (midnight)

## Name and GT user-id

Name: 
User ID:
Playcanvas Username (if appropriate): 

## Additional Details 

The goal of the assignment is to implement the HOMER interaction technique, and create a small test environment to use it in.  

You should satisfy the following constraints.

- create a space big enough to test the HOMER technique.  You could use either the Babylon default space or the Playcanvas space from the WebXR Sample.   
- distribute objects around it (cubes and other shapes, models, etc.).  Make sure there are a reasonable number of objects at different distances from you, and different sizes.
- use a physics engine and it's collision detection to enable you to raycast accurately against the objects regardless of their position and orientation.  (Both Babylon and Playcanvas make this relatively easy, and their are samples for both engines showing you how to do it.)
- use one controller to move around the scene (using whichever teleport and movement controls you want). You only need to move on the ground, not on objects.
- use the other controllers as your selection controller.  It should raycast and highlight the object selected (you could just change the color while selected, or use any other highlighting technique).  When the trigger is pressed and held, the HOMER technique should be used to rotate and move the selected object object as long as the trigger is held.

## Rubric

Graded out of 10.

1. Your exported project runs locally using `npm run start`. (1)
2. At least 10 objects of at least 3 types created around the scene of different sizes and distances from the user's starting point. (1)
3. Movement controls on one controller. (1)
4. Selection ray intersects objects correctly (using physics collisions) and highlights the closest object to the user that the ray intersects. (1)
4. Tip of controller model moves to intersection point when button pressed. (1)
5. Model rotates correctly as your rotate the controller. (1)
6. Model moves left, right, up, down correctly as you move that direction. (1)
7. Model moves using the correct linear scaling in and out as you move the controller closer or further. (2)
8. Model stays in the new position when the trigger is released, and can be selected and moved again. (1)

# Collaboration

You are free to discuss technical questions and issues in the Teams channels, but the code you submit should be your own.  So, please do not post large chunks of code, but providing pointers to examples or documentation pages or components and methods, along with discussion of how to use them, is fine.

# Submission

You will submit your assignment based on the instructions in 1(a), 1(b), or 1(c) (depending on if you used Babylon, Playcanvas Editor, or Playcanvas Engine, respectively.)

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Material for 3D User Interfaces Fall 2020</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.blairmacintyre.me/3dui-class-f20" property="cc:attributionName" rel="cc:attributionURL">Blair MacIntyre</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.

The intent of choosing (CC BY-NC-SA 4.0) is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Corsera, Udacity, LinkedIn Learning, and other similar sites).   