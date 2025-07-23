## Section 7: Audio In Unity

### 📌 Topics Covered  

1. Audio Source  
2. Singleton
3. Controling Audio Methods

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

- Simple App that plays and mutes the audio, and can switch to other scene without cutting off the audio.

---


### 🖼️ Screenshots  

<div align="center">

![Creating A Folder For Audio](https://i.imgur.com/PZ3UdV8.png)  
📌 *Created a folder for audio and placed the audio i wanna use inside of it.*

![Audio Source](https://i.imgur.com/YgahKoC.png)  
📌 *Created a game object and added an audio source component to it, then added an audio clip.*

![Adding Script](https://i.imgur.com/LDtnyoS.png)  
📌 *Added C# script to the camera*

![Load Scene Method](https://i.imgur.com/pHV8vUb.png)  
📌 *Wrote a method to move to the next scene*

![Aplpy Load Scene Method On Button](https://i.imgur.com/ZRPNfIp.png)  
📌 *Applied the load scene method on the button*

![](https://i.imgur.com/cf2WodZ.png)  
📌 **

![Moving To Other Scene](https://i.imgur.com/ijvJE54.gif)  
📌 *Now i can move to the other scene through the button, but the problem is the audio isn't playing in the second scene*

![Creating AudioObject Adding Audio Component + C# Script To It](https://i.imgur.com/youhUhD.png)  
📌 *Just created a gameObject called AudioObject and placed the scipt inside it instead of the camera then placed the audio copomemnt inside it too*

```
public static AudioManager _instance;

    void Awake()
    {
        if (_instance == null)
        {
            DontDestroyOnLoad(gameObject);
        }

        else
        {
            if(this != _instance)
            Destroy(gameObject);
        }
    }
```
![Code Effect](https://i.imgur.com/EOEDD1i.png)  
📌 *Now with this code, the audio moves with me to the next scene and it doesn't start from the begining.*

</div>

---

## Problems I Faced
* Audio didn't start playing in the other scene and the AudioObject didn't even appear, i went to the audio script turns out the problem was that i wrote awake() instead of Awake()

### 📁 Files / Assets Used
