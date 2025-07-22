## Section 7: Audio In Unity

### 📌 Topics Covered  

1. Audio Source  
2. Singleton

---

### ✍️ What I Learned

I learned about the **Audio Source** component in Unity. It allows you to play sounds in your game, like background music or sound effects.

- You can attach it to any GameObject.  
- Choose an audio clip to play.  
- Control playback settings like:  
  - Looping  
  - Volume  
  - Pitch  
  - Play on Awake

You can also control it through code:


audioSource.Play(); // Starts playing the sound  
audioSource.Stop(); // Stops the sound  


🛠️ **What I Did / Built**

- Created a folder for audio  
- Created an empty GameObject and added AudioSource  
- Wrote a script that plays the audio  
- Applied Singleton pattern to make audio persist between scenes  
- Connected the button to change scenes

---


### 🖼️ Screenshots  

<div align="center">

![Creating A Folder For Audio](https://i.imgur.com/PZ3UdV8.png)  
📌 *Created a folder for audio and placed the audio I wanna use inside of it.*

![Audio Source](https://i.imgur.com/YgahKoC.png)  
📌 *Created a game object and added an audio source component to it, then added an audio clip.*

![Adding Script](https://i.imgur.com/LDtnyoS.png)  
📌 *Added C# script to play the audio.*
