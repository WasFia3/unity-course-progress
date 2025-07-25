## Section 6: Advanced Unity Concepts

### 📌 Topics Covered  

1. Local and Global Position  
2. Local and Global Rotation  
3. Local and Global Space in Programming  
4. Rotation and Quaternions  
5. Cameras  
6. Light and Shadows  
7. Shaders and Materials  
8. MonoBehaviour Basics  
9. Awake and Start Methods  
10. FixedUpdate, Update, and LateUpdate  
11. Camera Positioning and Following  
12. Handling Input and Timers  
13. Releasing Control Over GameObjects  
14. Local Scale and LookAt  
15. Local Rotation and LookAt  
16. Vertical Rotation Using a Gun  
17. Coding Dots and Using Prefab Dots  
18. Raycasting and Testing  
19. Raycast Collision Detection Between Objects  
20. Creating a Dot Using Prefab  
21. Creating a Line Using a Prefab  
22. Creating a Line Prefab Through Code  
23. Creating a Multi-Line Prefab  
24. Coding a Drawing Game Using Multiple Lines  

---

### ✍️ What I Learned

I learned the differences between **local** and **global** position and rotation, and how the **space context** (self vs. world) affects object transformations in Unity. I also gained an understanding of **quaternions** and how they ensure smooth rotations.

Additionally, I explored **camera behavior**, **MonoBehaviour** methods like `Awake()`, `Start()`, and their roles in Unity’s update cycle. A key distinction is that `Awake()` executes even if the script is disabled, unlike `Start()`.

I also learned how **shaders** and **materials** work, how to **apply textures**, and how to implement camera mechanics such as **following the player** or creating an **FPS perspective**.
---

### 🛠️ What I Did / Built  

* Created and applied materials using imported textures.  
* Configured textures in the inspector.  
* Built a simple FPS-style camera system.  
* Tested MonoBehaviour methods in simple scripts.

---

### 🖼️ Screenshots  

<div align="center">

![Textures](https://i.imgur.com/kpssQdZ.png)  
📌 *Added texture to the project under the Textures folder.*

![Texture settings](https://i.imgur.com/XMw0hJA.png)  
📌 *Changed texture type to Default for use in materials.*

![Materials](https://i.imgur.com/vX9XqLJ.png)  
📌 *Created new materials from the Inspector.*

![Materials Applied](https://i.imgur.com/WSMpYe5.png)  
📌 *Applied the texture to create a new Brick and Box material.*

![Materials Applied To Objects](https://i.imgur.com/RZ5WYmP.png)  
📌 *Added some cubes to the scene with a plane that represents the ground and added material to each object.*


![Awake Start When Script On](https://i.imgur.com/5rvKvfQ.png)  
📌 *Both start and awake methods print on the consol while the scipt is on*

![Awake Start When Script off](https://i.imgur.com/Un22WPh.png)  
📌 *After turning off the script, we notice that only the awake method keeps working*

![Difference Between Update Methods](https://i.imgur.com/wC2pEqb.png)  
📌 *In Unity, 'Update()' is called once per frame and is used for non-physics-related logic like player input or basic movement. 'FixedUpdate()' runs at a consistent rate (usually every 0.02 seconds) and is meant for physics calculations like applying forces, ensuring accurate and stable results. 'LateUpdate()' runs after all Update() calls in the same frame and is useful for order-dependent logic—like making the camera follow the player after the player has moved.*

![Adding the camera to the cube](https://i.imgur.com/xEBISnV.png)  
📌 *Added the camera is a child of the cube, so it follows its position and rotation automatically, keeping a local offset.
Normally, we use transform.position + offset in LateUpdate() to follow the player smoothly, but parenting removes the need for code — Unity handles it each frame. *

![Camera following the cube](https://i.imgur.com/8Zi2TVP.gif)  
📌 *Now the camera succesfully follows the cube object*




</div>

---

### 📁 Files / Assets Used  

* Textures folder  
* Materials folder  
* Custom scripts for camera & movement  
* Test scene for MonoBehaviour methods  
