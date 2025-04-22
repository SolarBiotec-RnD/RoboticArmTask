# Box Balancing Challenge

## Overview
Welcome to the Box Balancing Challenge! This programming task is designed to test your problem-solving skills, algorithmic thinking, and code organization abilities. You'll be implementing a control system for a robotic arm that needs to balance boxes across multiple stacks.

## The Challenge

### Problem Description
You are working with a robotic arm in an automated factory. The arm can move left and right above a row of stacks, pick up boxes from the top of stacks, and place boxes it's holding onto stacks. Your task is to write an algorithm that will make the stacks as balanced as possible.

### What is a Balanced State?
- A set of stacks is considered balanced when the difference in the number of boxes between any two stacks is at most 1
- If the total number of boxes cannot be divided evenly, the extra boxes should be distributed from left to right
- Example: If you have 7 boxes and 3 stacks, the balanced state would be [3, 2, 2]

### Robot Arm Capabilities
The arm can perform four operations:
- `"LEFT"` - Move one position to the left
- `"RIGHT"` - Move one position to the right
- `"PICK"` - Pick up a box from the current stack
- `"PLACE"` - Place the held box on the current stack

### Constraints
- The robot arm can only hold one box at a time
- The robot arm can only pick from or place on the stack it's currently above
- Your solution must complete the task within 200 moves
- Stack sizes are non-negative integers
- The number of stacks can vary but will be at least 1

## Your Task

### What to Implement
You need to implement your solution into `solve` function in `task.py`. The function should return the next move for the robot arm based on the current state.

### Example
Initial state: `[3, 0, 0]`, claw at position 0, no box in claw
Desired final state: `[1, 1, 1]`
Possible solution: `["PICK", "RIGHT", "PLACE", "LEFT", "PICK", "RIGHT", "RIGHT", "PLACE"]`

## Getting Started

1. Make sure you have Python 3.7 or higher installed
3. Implement your solution in `task.py`
3. Run the tests:

   ```
   python run_tests.py or python3 run_tests.py
   ```

## Evaluation Criteria
Your solution will be evaluated based on:
1. Correctness - Does it successfully balance the boxes?
2. Efficiency - How many moves does it take?
3. Code Quality - Is the code well-organized, documented, and maintainable?
4. Error Handling - Does it handle edge cases gracefully?

## Testing
The simulator includes various test cases:
- Basic scenarios with 3-4 stacks
- Edge cases (empty stacks, single boxes)
- Complex scenarios with many stacks
- Special cases that test specific edge conditions

Each test will show:
- Output of initial and final states
- Number of moves taken
- Execution time
- Whether the test passed or failed


After you complete the task, upload your 'task.py' file using this google form link:

        https://docs.google.com/forms/d/e/1FAIpQLSdfAB64PSvXRMwE83kwLdN9khss5v93I2dQj3ImpxCkHhyYMg/viewform

Good luck with the challenge! We're excited to see your solution. 
