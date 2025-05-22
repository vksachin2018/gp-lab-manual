##EXP-04: Attach Rifle with character mesh and bullet spawn from Rifle.
## Date:9/4/25
## AIM:
To Attach Rifle with character mesh and implementation bullet spawn from Rifle .

## ALGORITHM(for attach rifle with character mesh):
```

1.	Import the rifle asset:	
•	Open your project in Unreal Engine.
•	Go to the Content Browser.
•	Right-click in the desired folder and select Import.
•	Locate and select your rifle asset file.
•	Configure the import settings as needed.
•	Click Import to bring the rifle asset into your project.
2.	Create a socket on the character mesh:	
•	Open your project in Unreal Engine.
•	Go to the Content Browser.
•	Right-click in the desired folder and select Import.
•	Locate and select your rifle asset file.
•	Configure the import settings as needed.
•	Click Import to bring the rifle asset into your project.
3.	Add the rifle to the character Blueprint:	
•	Open your project in Unreal Engine.
•	Go to the Content Browser.
•	Right-click in the desired folder and select Import.
•	Locate and select your rifle asset file.
•	Configure the import settings as needed.
•	Click Import to bring the rifle asset into your project.
4.	Adjust the rifle's position and rotation:	
•	Open your project in Unreal Engine.
•	Go to the Content Browser.
•	Right-click in the desired folder and select Import.
•	Locate and select your rifle asset file.
•	Configure the import settings as needed.
•	Click Import to bring the rifle asset into your project.
5.	Test the attached rifle:
•	Open your project in Unreal Engine.
•	Go to the Content Browser.
•	Right-click in the desired folder and select Import.
•	Locate and select your rifle asset file.
•	Configure the import settings as needed.
•	Click Import to bring the rifle asset into your project.

```
## OUTPUT:
## GUN ATTACHED TO PLAYER:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/1aca6c2a-257a-40dc-ac53-483280d9089e)

  
## GUN ACTOR SPAWN:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/375fdce6-b59b-476d-8fc9-d8f8491ba109)

 

## STATE GRAPH:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/c45fb333-8c5a-4254-a8fa-defcc06d7fcf)
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/097d5d68-a899-4563-9ce1-8c10ca25c31b)

 

 
 
## IDLE TO GUNIDLE:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/88e66115-9f7b-4dcd-805f-b09634109bc9)

 
## GUNIDLE TO IDLE:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/d3d3e9b4-2c9b-4edb-9e2f-4dd71903912c)

 
## GUNIDLE TO GUNRUN:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/88c1bde8-8d48-401a-af1e-c73d056259d5)

 
## GUNRUN TO GUNIDLE:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/d529372d-89ee-4b51-a9e9-a603c3c531ff)


  
## INPUT ACTION TO EQUIP THE GUN:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/5a9110f8-f2c3-4a08-b74f-033846396238)
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/c99ad8c6-1b4a-476a-bec3-942b2c16aaa8)

 
 
## GUN EQUIP:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/a6c1b370-dd7d-4e93-bfe3-6165fb4a2eaf)


  
 

## ALGORITHM(for implementing bullet spawn from rifle):

1.	Create a bullet projectile:
•	In the Content Browser, right-click in the desired folder.
•	Select Create Basic Asset > Blueprint Class.
•	In the Class Settings window, search for "Projectile" and select it as the parent class.
•	Name the Blueprint (e.g., "BulletProjectile") and click Create.
2.	Set up the bullet projectile:
•	Open the BulletProjectile Blueprint.
•	In the Blueprint editor, locate the Components panel on the left.
•	Add a Static Mesh component to represent the visual representation of the bullet.
•	Adjust the Static Mesh component's properties as desired (e.g., mesh, scale, materials, etc.).
•	Add any other necessary components (e.g., collision, audio, particle effects) to enhance the bullet's behavior.
3.	Set up the rifle Blueprint:
•	Open the rifle Blueprint that is attached to the character (refer to the previous steps on attaching the rifle).
•	In the Blueprint editor, locate the Event Graph tab.
•	Find the event that triggers the firing action (e.g., "Fire" button press).
•	Create a new custom event node for spawning the bullet projectile.
•	Drag off the custom event node and search for "Spawn Actor from Class".
•	Connect the execution line from the event node to the Spawn Actor node.
4.	Configure the Spawn Actor node:
•	In the Spawn Actor node, select the BulletProjectile Blueprint as the Class.
•	Connect the execution line from the Spawn Actor node to any necessary nodes or logic related to the firing action (e.g., setting the bullet's initial velocity, applying recoil to the rifle, playing firing sound).
5.	Adjust the spawn location and rotation:
•	Drag off the Spawn Actor node and search for "Get Socket Transform".
•	Select the character's rifle socket (the socket where the bullet should spawn).
•	Connect the output of the Get Socket Transform node to the Spawn Transform input of the Spawn Actor node.
6.	Test the bullet spawning:
•	Compile and save the rifle Blueprint and BulletProjectile Blueprint.
•	Play the game to test the character's firing action.
•	Ensure that when the firing action is triggered, the bullet projectile is spawned from the rifle's socket with the desired behavior.
 
## OUTPUT:
## ARROW FUNCTION:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/41b00164-91a1-48ec-9721-cec2c8d6bd16)


 
## BULLET ACTOR:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/92175a25-4230-4f70-aa5c-67244efd0de8)

 

## BULLET SPAWN:
![image](https://github.com/Prethiveerajan/Unreal-EXNO-04-Attach-Rifle-with-character-mesh-and-implementation-bullet-spawn-from-Rifle-/assets/94233064/c1516adc-8962-40b7-aa54-c41e5f00ac1e)


 

## RESULT:
Thus, Rifle is Attached with character mesh and implementation bullet spawn from Rifle is done 
 











































