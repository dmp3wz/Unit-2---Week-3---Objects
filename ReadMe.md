# Unit 2 - Week 3 - Objects

## Slides
https://myuva-my.sharepoint.com/:p:/g/personal/jcb2h_virginia_edu/ESjYUJDLpExOqvlfpCVEijYBfPAoCXWpdUT7LpooCv_Xjw?e=ZIzakb

## Relevant Manual Pages

https://docs.unity3d.com/Manual/GameObjects.html

https://docs.unity3d.com/Manual/PhysicsOverview.html

https://docs.unity3d.com/Manual/Lights.html

## Skills
* GameObject types (refresher)
* The Transform Component
* Enabling / Disabling GameObjects and Components
* World vs Local Space
* 3D Objects / Meshes / Mesh Filter
* Rendering / Mesh Renderer / Materials
* Lights
* Colliders
* Rigidbodies
* Joints
* The Rectangle Tool
* Sketchfab

## Level
1. Open "First Person Scene"
2. Create a hallway with a floor, walls, and a roof
3. Create a room at the end of the hallway (try to do this *efficiently*)
4. Make a stack of boxes at the end of the hallway, such that your player has to smash through  them, Kool-Aid Man-style
5. Build a swinging pendulum that does the same

NOTE: Your player uses standard keyboard FPS controls, which are as follows:

**W,A,S,D keys** = forward, left, back, right

**Mouse** = rotate view

**Space** = Jump

## Bosses

### Bowser
<img src="https://user-images.githubusercontent.com/7291792/187090817-9c0523ad-2e40-4760-8f93-b92516b64b7f.png" width=200/>
A game designer sends you an email for a game element with this story: 
Your character walks down a long hallway into a room. They see shadows on the walls in the room. On the floor is text telling them to "stand here" and a dot on the floor. When they stand there, the shadows resolve into text that gives them a clue to a puzzle on how to leave the room.
<br/><br/>

Assets: use the provided 3D Text models in Assets > Art > 3D Models as your text object(s)
(NOTE: if you want to make your own 3D text, you'll need to get the program Blender, which is free, and follow the first two steps of this guide: https://www.makeuseof.com/3d-text-in-blender-how-to/ and export the model as an FBX file into your Assets folder via File > Export > FBX in Blender)


Special conditions for the puzzle: in the Scene (and therefore the start of the Game), there are no lights in the room with the 3D text (nor a light object near enough to cast any shadows); how is it your character (while playing the game) can see shadows on the walls?

HINT: To write on the floor, use a particular kind of GameObject...

### Hornet
<img src="https://user-images.githubusercontent.com/7291792/187090928-364593f1-da58-46bc-a4a5-e777fd46fdd2.png" width=200/>
After the player escapes the room, they must jump between a series of swinging platforms. Use Triggers to activate some of the elements in the Scene.
https://docs.unity3d.com/ScriptReference/Collider.OnTriggerEnter.html
https://docs.unity3d.com/ScriptReference/Collider.OnTriggerExit.html

### Demon of Hatred
<img src="https://user-images.githubusercontent.com/7291792/187091229-df150009-ed6c-4d7b-8640-3c79fa270cbd.png" width=200/>

Do the above challenges, but build it all with the ProBuider package instead of primitives. 


BONUS: Instead of boxes in Level part #4, make a REALISTIC stack of traffic cones (that is, they should stack as cones naturally stack)

Add in a new game element of your choosing.
