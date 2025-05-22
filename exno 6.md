# EXP-06: Implement the AI random movement.
## Date: 24/4/25

## Aim:
Implement the AI random movement.

## Algorithm:
- Step:01 Create a Character Blueprint.
- Step:02 Create a Blackboard.
- Step:03 Open the Behavior Tree editor.
- Step:04 Create Behavior Tree nodes for the following:

    "Selector" node: Controls the execution of child nodes.  
    "Service" node: Monitors and updates values in the Blackboard.  
    "Sequence" node: Executes child nodes in sequential order.  
    "Random" decorator: Randomly selects a child node to execute.  
    "Move To" task: Moves the AI character to a specified location.

- Step:05 Set up the Blackboard with vector key and bool keys and save it.
- Step:06 Set up the AI character Blueprint with the help of AI controller component.
- Step:07 Set the AI controller and behavior treeiIn the Possess node, select the AICharacter Blueprint you created and drag off the AICharacter reference and search for “Use Blackboard”
- Step:08 Set up the NavMesh and boundaries, we can adjust the size and position to cover the desired play area.

## Output:

![image](https://github.com/user-attachments/assets/23562410-300b-408f-8e9c-e4c3a9ea7037)

![image](https://github.com/user-attachments/assets/ae6737ed-0930-4580-a571-048622117929)

![image](https://github.com/user-attachments/assets/d53b8f65-89ee-4099-af6c-2f2aa92e1744)


## Result:
Thus, the AI concept to the actor for a random movement is imple
