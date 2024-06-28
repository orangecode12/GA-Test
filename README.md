## Genetic Algorithms (Test task)

### Task:
A van in a shop must be filled to transport household appliances, its load must be optimized by maximizing the value of what is transported for a given volume. 

### Solution Overview:
The primary challenge encountered in the project was the development of an effective fitness_func. The initial approach involved returning a tuple comprising two distinct elements: fitness_value and fitness_space. However, this strategy proved to be suboptimal due to the significant disparity in their respective ranges, which led the optimization algorithm to predominantly focus on the fitness_value, thus neglecting the fitness_space.

To address this, the logarithmic function was employed to normalize the ranges, thereby enabling the algorithm to concurrently optimize both fitness metrics. Further refinements included adjusting the parameters for pygad.GA(). A notable issue was the occurrence of errors when both fitness values were zero. To mitigate this, a small constant was introduced to prevent zero values.

Although my expertise in Genetic Algorithms (GA) is still developing, the implemented solution appears to be functioning effectively. Continuous learning and experimentation are anticipated to enhance the robustness of the solution further.

### Solution Usage:
It is possible to use this solution for all free_space values between 1 and 5, just change the variable in the very begining of the code.
