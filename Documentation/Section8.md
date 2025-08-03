## Section 8 UI Desgin and Animation + Events basics

### 📌 Topics Covered  
1. Importing pictures and responsive background
2. Canvas/ rect transform/ center point/ pivot
3. Anchors and best fit
4. Dealing with responsive images / buttons / pannels / texts
5. Dealing with menus
6. Vertical slider.
7. Slider mask
8. Menu buttons / opening and closing the menu
9. Animation 


---

### ✍️ What I Learned
* We call the folder that contains the images in the game "Sprites". 
* Learned about responsive component, to take the full screen change Xscalefrac to .2 Yscalefrac to .3.
* sprite renderer component
* Any object inside the canvas should be from "Rect Transform" type.
* We usually resize the width and height to change the UI object size, so it stays responsive. we do not use scale for that.
* Anchors are reference points that control how UI elements behave when the screen size or resolution changes. They’re part of the RectTransform component used in UI.
* Sprite sheet is a single image file that contains multiple smaller images (sprites), usually used for animations or game objects.
* Scroll Rect component
* Rect 2D Mask component
* Animator component



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

![Multiple Sprite](https://i.imgur.com/zJZVNIR.png)  
📌 *Multiple sprite mode*

![Multiple Sprite](https://i.imgur.com/cJD0x6Q.png)  
📌 *Multiple sprite edit*


![Vertical layout group](https://i.imgur.com/YPCdXBK.png)  
📌 *Vertical layout group component applied on menu to group the buttons inside the menu*

![Menu children](https://i.imgur.com/SsGxFT3.png)  
📌 *Buttons inside the menu*

![Final](https://i.imgur.com/JweY6HH.png)  
📌 *Final layout*

![Scrol Rect](https://i.imgur.com/zPEuVnM.png)  
📌 *Created an empty game object and placed the menu inside it as a child, then added this component to it to make the menu slide vertically*

![Scrol Rect](https://i.imgur.com/MbNIl8H.gif)  
📌 *The final result after adding the scroll rect component*

![Mask rect](https://i.imgur.com/kwyAGOC.png)  
📌 *Added mask to the menu*

![Result after mask](https://i.imgur.com/QYOP7LS.gif)  
📌 *Final result after adding the mask*



</div>

---


  ### 🧪 Problems I Faced  
* The events.cs class had error "The type or namespace name 'Mindizor' could not be found (are you missing a using directive or an assembly reference?)CS0246", i created a LinkHolder.cs to solve the problem
  ![LinkHolder](https://i.imgur.com/93wKghT.png)  
📌 *LinkHolder Class.*

  ![Events](https://i.imgur.com/6CGGfnj.png)  
📌 *Events Class.*

* Responsive attrubites won't appear, restarted unity and it worked.
* When implementing a vertical/horizontal scroll view using Unity’s Scroll Rect component, the scroll content moves correctly during drag, but once the mouse/finger is released, the content immediately snaps back to its original position instead of staying at the new scroll offset.

  ![Slide problem](https://i.imgur.com/IScBTsL.png)  
📌 * I fixed this problem by changing the movment type from "Elastic" to "Unrestricted".*
