# CVFX-homework-5
## 1. Motion Parallax
### multi-view images
先在校門口拍了張照片，然後往旁邊走一步再拍一張。

圖1：

<img src="https://i.imgur.com/T4qfsBG.jpg" width="300">

圖2：

<img src="https://i.imgur.com/ShcH9uM.jpg" width="300">

### image alignment results
為了使照片裡的國立清華大學盡量保持不動，所以我們只使用了照片中間部分來找match points，然後再把得到的homogrophy matrix對整張圖片進行處理，最後得到這張圖3。

圖3：

<img src="https://i.imgur.com/EZDo0IF.jpg" width="300">

### multi-view 3D visual effects

origin(圖1+圖2)：

![](https://i.imgur.com/oemIe4M.gif =300x)

motion parallax(圖3+圖2)：

![](https://i.imgur.com/b4VOxkP.gif =300x)


## 2. Stop motion
### multi-view images

![](https://i.imgur.com/81vlFAG.png)

Stop Motion的部份我們決定拍不同角度的沉思者
以上是我們由右往左拍的結果

### image alignment results
![](https://i.imgur.com/aioEz60.png)
![](https://i.imgur.com/6VM5l7f.png)

在align的時候我們將所有圖片段同一張圖做align,
也就是最中間的那一張圖，這樣整個相機的視角才會一致
如此一來就能去除在拍攝過程中的晃動

### multi-view 3D visual effects
original:

![](https://i.imgur.com/OAFsLGH.gif)

stop motion:

![](https://i.imgur.com/JnUa8gN.gif)

我們可以明顯看得出來align前整個影片看起來非常地晃，
可是align就變得非常滑順，有stop motion的感覺。
但是align後的影片在最右跟最左邊的石像都出現了歪斜。

## 3. Live photo
### multi-view images
![](https://i.imgur.com/PpbgXI0.jpg)

Live photo主要為拍攝國旗飛揚，但從不同的照片中，可以發現因為不同的時間，國旗飛揚的面積大小不同，每張拍攝角度也稍有偏差。

### image alignment results
由於我們希望背景盡量是一致的，讓國旗飛揚的效果更加明顯，
因此我們將所有照片都align在第一張，使其他照片視角與第一張一致，
以下是align之後的比較圖。

![](https://i.imgur.com/YUCm1q8.jpg)

從上圖可以得知，有些照片因為手持的角度不同，導致旗竿非完全直立，
經過align以後，將旗竿調整成原本的直立效果，並保持背景一致。

### multi-view 3D visual effects
以下為原圖與Live Photo的比較。

* Original

![](https://i.imgur.com/Lpid6gA.gif)

* Live Photo

![](https://i.imgur.com/jx8N8mx.gif)

由於align以後，外圍會出現變形的情況，因此我們將align後的圖片，去掉變形的部分。

由上圖的比較可以發現原本的圖片，因為手持的關係有不同角度的歪斜，但下圖經過align後，背景明顯的較為一致，只有國旗在飛揚。



## 4. Effect enhancement

* Stop-motion
我們在沉思者上面加了濾鏡，讓整個沉思者的色調變暗，
營造出更有沉思的氣氛。

![](https://i.imgur.com/sP7fa9Q.gif)

* Live Photo
為了更凸顯國旗飛揚的效果，我們加上超人，使觀眾的目光都聚集在超人上，減少對其他景物的注意，並以國旗作為超人的披風，成為超人飛翔的Live Photo。

![](https://i.imgur.com/b2lrYXu.gif)






