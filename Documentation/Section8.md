## Section 8 UI Desgin and Animation + Events basics

### 📌 Topics Covered  
1. Importing pictures and responsive background
2. Canvas/ rect transform/ center point/ pivot
3. Anchors and best fit
4. Dealing with responsive images / buttons / pannels / texts
5. Dealing with menus 


---

### ✍️ What I Learned
* We call the folder that contains the images in the game "Sprites". 
* Learned about responsive component, to take the full screen change Xscalefrac to .2 Yscalefrac to .3.
* sprite renderer component
* Any object inside the canvas should be from "Rect Transform" type.
* We usually resize the width and height to change the UI object size, so it stays responsive. we do not use scale for that.
* Anchors are reference points that control how UI elements behave when the screen size or resolution changes. They’re part of the RectTransform component used in UI.
* Sprite sheet is a single image file that contains multiple smaller images (sprites), usually used for animations or game objects.



---

### 🖼️ Screenshots  

<div align="center">

![Background](https://i.imgur.com/OpIA4r9.png)  
📌 *Added responsive script to the background*

![Before](https://i.imgur.com/AE6bLTn.png)  
📌 *Before starting the game mode*

![After](https://i.imgur.com/XEneGX8.png)  
📌 *After starting the game mode*


![Anchors](https://i.imgur.com/x78btNK.png)  
📌 *Anchors for button*


</div>

---


  ### 🧪 Problems I Faced  
* The events.cs class had error "The type or namespace name 'Mindizor' could not be found (are you missing a using directive or an assembly reference?)CS0246", i created a LinkHolder.cs to solve the problem
  ![LinkHolder](https://i.imgur.com/93wKghT.png)  
📌 *LinkHolder Class.*

  ![Events](https://i.imgur.com/6CGGfnj.png)  
📌 *Events Class.*

* Responsive attrubites won't appear, restarted unity and it worked.
