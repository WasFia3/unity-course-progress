## Section 11: Basics of Game Development and Programming

### 📌 Topics Covered  
1. How to import sprites properly.  
2. Creating the player and its animation.  
3. Adding objects and background.  
4. Adding collision and physics-affected objects to game entities.  
5. Adding player and game logic features + sound effects.  
6. Adding movement to the game and implementing grounded detection.  
7. Adding a score system via collision and displaying it using TextMesh.  
8. Expanding the world, moving it, and adding death zones to the game.  
9. Adding jump effects to the player with movement effect parameters.  
10. Coding jump states using time delay.  
11. Adding win points to the game.

---

### ✍️ What I Learned

- If working with a mobile device app, change the sprite format to **TrueColor** to avoid pixelated images.  
- Learned about the **Sprite Renderer** component.  
- You can place the background behind the object by switching to **3D Mode** and moving the background backwards along the **Z-axis**.

---

#### 🏷️ Tags in Unity
- Tags are labels you assign to GameObjects.  
- Used to identify objects in code.

#### 🧅 Layers in Unity
Layers are used for:
- Collision filtering (with the Layer Collision Matrix)  
- Camera culling (what each camera sees)  
- Raycasts (to hit only specific layers)

---

### 🛠️ What I Did / Built  
*Added animated sprites, implemented movement, collisions, gravity, and began organizing object layers and tags.*

---

### 🖼️ Screenshots  

<div align="center">

![Animation](https://i.imgur.com/PaI7Wm6.gif)  
📌 *Added a sprite to the scene, then animated it with a simple blinking animation.*

![Adding collider + rigidbody](https://i.imgur.com/49wK3Rs.png)  
📌 *Added two components to the player:*  
- *Rigidbody2D so the player is affected by gravity*  
- *Box Collider 2D for collision detection*

![Tags and layers](https://i.imgur.com/G7B4ocf.png)  
📌 *Created a tag for the coin to identify it in code when the player touches it.*  
*Created a layer for the ground so physics checks (like grounded detection) only interact with ground objects.*

![Is triggered for coin](https://i.imgur.com/YJ81LUO.png)  
📌 *Enabled "Is Trigger" on the coin so the player can pass through it and still detect the collision to collect it.*

![Result 1](https://i.imgur.com/0wIBDz4.gif)  
📌 *Final result after managing collisions, gravity, and enabling "Is Trigger" on the coin.*

![Result 2](https://i.imgur.com/0wIBDz4.gif)  
📌 *Final result after adding the score variable to display the player's coin count. Now, when the player touches a coin in the game, the coin count increases and the updated score is shown on the screen using the TextMesh.*

![World object](https://i.imgur.com/6Tq2zsV.png)  
📌 *Created a world object that contains the ground objects and coins, so I can animate the world later.*

![DeadZone](https://i.imgur.com/9271WYM.gif)  
📌 *Result after animating the world and adding a deadzone.*

![Jumping parameters](https://i.imgur.com/CiTIClv.png)  
📌 *Created triggers in the Animator to help track the jumping process.*

![Transactions](https://i.imgur.com/IkaBjd6.png)  
📌 *The Animator shows two states: `PlayerAnimation` (idle/move) and `JumpAnimation`. When the `jumped` trigger is activated, it transitions from `PlayerAnimation` to `JumpAnimation`.*

![Jumping result](https://i.imgur.com/ofpAEcv.gif)  
📌 *Player jump animation with delay before landing, triggered using grounded check and upward force.*

</div>

---

### 📁 Files / Assets Used  
- **Sprites:**
  - Player sprite sheet (idle, blink, jump frames)  
  - Coin sprite  
  - Ground tile sprite  
  - Background sprite  

- **Audio:**
  - `Jump.wav` — jump sound effect  
  - `Coin.wav` — coin collection sound effect  
  - `Win.wav` — win sound effect  

- **Scripts:**
  - `controllerPlayer.cs` — handles player movement, jumping, collisions, and score  
  - Scene setup files (`Section11.unity`)

---

### 🧪 Problems I Faced  
- The sprite wasn't appearing on the camera — turned out its **Z-axis was -10**, so I changed it to **0**, and it started appearing correctly.

---
