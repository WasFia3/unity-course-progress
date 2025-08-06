## Section 11 Basics of game development and programming

### 📌 Topics Covered  

1. How To Import Sprites Properly.
2. Creating The Player And Its Animation.
3. Adding objects and background.
4. Adding Collision and Physics-affected Objects to Game Entities.
5. Adding Player and Game Logic Features + Sound Effects
6. Adding Movement to the Game and Implementing Grounded Detection
---

### ✍️ What I Learned
* If working with a mobile devide app, change the sprites format to TrueColor to avoid getting pixeled pixtures.
* Sprite Renderer component
* We can place the background behind the object by switching to 3D mode and moving the background backwards along the Z-axis.
  ---
* 🏷️ Tags in unity:
*Tags are labels you assign to GameObjects.
*Used to identify objects in code.

🧅 Layers:
Layers are used for:

*Collision filtering (with Layer Collision Matrix)
*Camera culling (what each camera sees)
*Raycasts (to hit only specific layers)

--- 
### 🛠️ What I Did / Built  


---

### 🖼️ Screenshots  

<div align="center">

  ![Animation](https://i.imgur.com/PaI7Wm6.gif)  
📌 *Added sprite to the scene then animated it simple blinking animation*

  ![Adding collider + rigibody](https://i.imgur.com/49wK3Rs.png)  
📌 *Added two components to the player, first one is rigibody 2D, so the player becomes effected by the gravity.*
    * Secind compenent is box collider 2D, for the collisions.*



</div>

---

### 📁 Files / Assets Used  

* Textures folder  
* Materials folder  
* Custom scripts for camera & movement  
* Test scene for MonoBehaviour methods

---

### 🧪 Problems I Faced  
* The sprite wasn't appearing on camera, turns out Z axis was -10 for that sprite, changed it to 0 and it started appearing on camera.
