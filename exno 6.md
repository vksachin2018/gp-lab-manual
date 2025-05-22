EXP-06: Implement the AI random movement.
Date:24/4/25
Aim
To implement an AI character in Unreal Engine that roams randomly within a defined area using Behavior Trees and Navigation Mesh.

Procedure
Navigation Setup

Add a NavMeshBoundsVolume to your level and scale it to cover the roamable area.
Ensure navigation is built (press P to visualize the navmesh).
Create AI Character

Create a new Character or Pawn Blueprint (e.g., BP_AICharacter).
Add an AIController Blueprint (e.g., BP_AIController) and assign it to your AI character.
Set Up Behavior Tree

Create a Behavior Tree (e.g., BT_RandomRoam) and a corresponding Blackboard.
Add a Blackboard Key (e.g., TargetLocation) of type Vector.
Implement Roaming Logic

In the Behavior Tree, use the following structure:
Root ➝ Selector
Sequence
Find Random Location (custom task to set TargetLocation)
Move To node (uses TargetLocation)
Create a custom BTTask Blueprint for finding a random location using UNavigationSystemV1::GetRandomPointInNavigableRadius.
Place and Test

Place your AI character in the level.
Assign the AI Controller and Behavior Tree.
Play the scene and observe the AI roaming randomly.
Output
Screenshot 2025-05-08 221444

image

image

image

image

Result
The AI character successfully roams within the defined NavMesh area, choosing random destinations at intervals using the Behavior Tree logic.
