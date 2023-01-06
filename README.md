
# The problem

Functions can only have a single y coordinate for every x value. However, what if we want to draw paramtric curves (i.e. curves that have multiple y-coordinates for a single x value):

<img width="581" alt="image" src="https://user-images.githubusercontent.com/59632554/211046128-e2fb2391-3198-44bb-8163-d4fb307e049d.png">

# ParametricCurveDrawing

This program will create and display parametric curves representing three-letter word of your choosing in bubble-like style


## Implementation Details - Python's spline and plotting functionality
* Ginput - to accept mouse-clicks on a blank figure, terminate when ginput is 0
* For each input curve date we: 
  1)  Create a piecewise linear plot of the current set of points
  2) Construct an approcimate arc-length paraetirixaitn t from the points
   <img width="526" alt="image" src="https://user-images.githubusercontent.com/59632554/211046039-29a4e53e-cea6-4e05-bf57-647f39752e20.png">
   <img width="306" alt="image" src="https://user-images.githubusercontent.com/59632554/211048394-de8a1062-ce3b-4bd3-a0a9-18435a985914.png">
  
  3) Construct two spline objects for X and Y coordintes sperately with respective arc-length parametrization [**make_interp_spline(x,y,cond)**]
  4) Plot the resulting splines
  
# Result:

**Figure A - The Original User Input**

<img width="818" alt="image" src="https://user-images.githubusercontent.com/59632554/211047677-46935e2f-3fdf-4cc9-80a1-7dfbfb4fe919.png">

**Figure B - Smooth Spline Plot**

<img width="819" alt="image" src="https://user-images.githubusercontent.com/59632554/211046856-085f476b-d260-4abe-88a6-1e0df9f33a95.png">

  
  
 


  
