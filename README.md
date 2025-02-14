# Ruby Instance Variable Modification Bug

This repository demonstrates a common, subtle error in Ruby related to how instance variables are accessed and modified.  The `bug.rb` file shows the incorrect approach to changing an instance variable's value, while `bugSolution.rb` provides the correct solution.

**Problem:**  In Ruby, you cannot directly assign a new value to an instance variable using the getter method.  This attempts to set the return value of the getter which will have no effect on the instance variable. 

**Solution:** Use a setter method (or modify the instance variable directly) to update the instance variable's value.