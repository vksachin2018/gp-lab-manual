EXP-02: Create A Player Movement Using Pawn, Collectable, Player Health And Score.

Aim:
To Create a player movement using pawn, collectible, player health and score.

Procedure To Create and Destroy the coin:
1. Create a new project in Unreal Engine and choose a template that suits your needs.
2. Add a new actor to the level and call it "Coin".
3. Create a new blueprint based on the Coin actor by selecting it in the Content Browser and
choosing "Create Blueprint".
4. Open the Coin blueprint and add a static mesh component to represent the coin. You can
import a 3D model or use one of the default shapes provided by Unreal Engine.
5. Add a collision component to the Coin blueprint so that the player can interact with it.
Choose a simple collision shape like a sphere or a box.
6. Add a collision component to the Coin blueprint so that the player can interact with it.
Choose a simple collision shape like a sphere or a box.
7. Create a new blueprint based on the player character by selecting it in the Content
Browser and choosing "Create Blueprint".
8. Open the player blueprint and add a collision component to represent the player's
interaction with the coins.
9. Add an event to the player blueprint that gets triggered when the player collides with a
coin. Use a collision event and check if the collided actor is a coin.
10. If the collided actor is a coin, check if it has already been collected. If not, set its
IsCollected variable to true and add its value to a score variable in the player blueprint.
11. Remove the coin from the level by calling its Destroy function.
12. Add several instances of the Coin actor to the level and adjust their positions so that they
are spread out and not too close to each other.

Output:
//paste your output screenshot here

Procedure To Redirect to levels:
1: Create a new level or open an existing one.
2: Add a new widget blueprint by going to the Content Browser and right-clicking in the
desired folder. Select User Interface and then Widget Blueprint.
3: Design your menu by adding buttons and other UI elements to the widget. You can use
images, text, and other widgets to create a visually appealing menu.
4: Add a button to your menu by dragging and dropping a Button widget from the Paletteonto
your canvas.
5: In the Button's properties, scroll down to the On Click section and click the + button next to
the On Click event.
6: Create a new custom event by clicking the New Binding button and selecting Custom
Event.
7: Name the custom event "LoadScene" or something similar.
8: Open the Level Blueprint by going to the Blueprint menu and selecting Open Level
Blueprint.
9: Drag and drop your menu widget from the Content Browser into the Level Blueprint.
10: Create a new variable in the Level Blueprint by clicking the Add Variable button in the
MyBlueprint panel. Name the variable "MenuWidget" or something similar and set its type to
the widget blueprint you created earlier.
11: In the Level Blueprint, drag from the MenuWidget variable and select Set to set the
variable's value to the instance of the menu widget you added to the level.
12: Create a new function in the Level Blueprint by clicking the Add Function button in the
My Blueprint panel. Name the function "LoadScene" or something similar.
13: Drag from the MenuWidget variable and select Get to get the instance of the menu
widget.
14: Drag from the Get node and select Remove From Parent to remove the menu widget from
the screen.
15: Drag from the LoadScene custom event and select Open Level to open the desired level
or scene.
16: Connect the nodes in the LoadScene function as follows: LoadScene -> Remove From
Parent -> Open Level.
17: Go back to your menu widget and select the button you added earlier.
18: In the Button's properties, scroll down to the On Click section and select the LoadScene
custom event you created earlier.
19: Save your changes and playtest your game. When the player clicks on the button in the
menu, the menu widget will be removed and the desired level or scene will be loaded.

Output:
//paste your output screenshot here

Result:
Thus, To Create a player movement using pawn, collectible, player health, and score created and
developed by unreal Engi