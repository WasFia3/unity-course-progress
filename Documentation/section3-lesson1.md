# Section 3 (whole)

### 📌 Topics Covered  
1. What is Unity Playground?
2. Downloading and Running Unity Playground Inside the Project
3. Adding Polygon collider and Attaching the Camera to the Player
4. Adding Health System and Health-Affecting Characters
5. Adding Coins / Collectible Currency
6. Game Ending and Making the Player Win
7. Adding Music, Sound Effects, and Audio Mixer
8. Downloading the Lesson Project
8. Creating Game Levels and Making the Player Jump and Reach the Platform

###  ✍️ What I Learned  

Everything starts with the assests folder, it's the heart's project, that's where you place all the project's content:C# scripts, sprites, animations, prefabs, audio files, materials, and UI elements...

- Cpmponents
I learnt about the assests's components, A component in Unity is like a behavior or ability that you attach to a GameObject to make it do some action.

I focused on these components:
* Rigidbody : This component gives your GameObject physics. Like, actual gravity, momentum, forces
* polygon collider: This component defines the shape of your object for collisions — but in a very detailed, custom way. it's represented in a green square.
* move : This component handles the movement logic of a GameObject.

- 📄 Scripts 

Scripts in Unity are components written in C# that define the behavior of GameObjects.

I focused on these scripts:
* Follow target: A script you attach to the camera (or a camera controller object) that makes it follow a specific target, usually the player, during gameplay.


  
### 🛠️ What I Did / Built  



### 🧪 Problems I Faced  
* Low disk storage
* Wasn't able to open the project provided by the instructor because it's built with an older version of Unity.
* Polygon collider didn't work due to forgetting to turn off the background (playground --> turn off background).
* The movment of the player was way too fast, solved this issue by increasing the mass property in the Rigidbody component.
* The player would keep falling, fixed this issue by freezing the movment on the z axis.

### 🖼️ Screenshots  

### 📁 Files / Assets Used 

### 💡 Notes / Tips  
