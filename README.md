# path-planning-ode

This is my revamped code for solving the autonomous path planning problem outlined at https://www.youtube.com/watch?v=fNBrIngCJp8&t=9s

## REQUIREMENTS:

-numpy
-sympy
-matplotlib

## MODULE USAGE:

The main API is the PathPlanningODE class. 

>>> pp_instance = PathPlanningODE(startingcoordinate (tuple, optional), endingcoordinate (tuple, optional)) to create instance of class

>>> pp_instance.create_obstacles(number_of_obstacles) to create multiple obstacles at once - default 10

>>> pp_instance.create_obstacle((xcoordinate, ycoordinate)) to create obstacle at specific location

>>> pp_instance.update_path() to iterate Newton's Method

>>> pp_instance.show_solution() to display current results

>>> pp_instance.animate_solver() to show animation of ODE solver in progress

>>> pp_instance.animate_rover() to show animation of rover following path

>>> pp_instance.Path.path to access x & y coordinates of solution path

