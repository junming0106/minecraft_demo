# Minecraft MakeCode｜生出 10 隻雞（拆解教學）

## Step 1: 先放一個「一開始就做」的框框
進入 Minecraft 世界時，程式就會開始動。  
我們先把動作放進「一開始」裡面。  
現在先不做事也沒關係，先把位置準備好。  

```blocks
```

## Step 2: 先試試看生出 1 隻雞
加入「生出動物」這個積木。  
CHICKEN 就是「雞」。  
先讓世界裡出現 1 隻雞，看看有沒有成功。  

```blocks
// 一開始
mobs.spawn(CHICKEN, pos(0, 0, 0))
```

## Step 3: 看懂 pos(0, 0, 0) 是哪裡
pos(0, 0, 0) 是一個「固定座標」。  
0, 0, 0 的意思是：角色的原點。  
所以每次雞都會在玩家腳底下生出來。  

```blocks
// 一開始
mobs.spawn(CHICKEN, pos(0, 0, 0))
```

## Step 4: 讓它重複做 2 次
加入「重複」積木，叫它做很多次。  
數字 2 的意思是：做 2 次。  
你會看到雞變成 2 隻，而且都擠在同一個地方。  

```blocks
// 一開始
for (let index = 0; index < 2; index++) {
    mobs.spawn(CHICKEN, pos(0, 0, 0))
}
```

## Step 5: 把次數改成 9 次
把重複的數字改大一點。  
9 的意思是：做 9 次。  
你會看到雞更多了，畫面會變得很熱鬧。  

```blocks
// 一開始
for (let index = 0; index < 9; index++) {
    mobs.spawn(CHICKEN, pos(0, 0, 0))
}
```

## Step 6: 完成 10 次，生出 10 隻雞
最後把 9 改成 10。  
10 的意思是：做 10 次。
```blocks
// 一開始
for (let index = 0; index < 10; index++) {
    mobs.spawn(CHICKEN, pos(0, 0, 0))
}
```



> 在 [https://junming0106.github.io/minecraft_demo/](https://junming0106.github.io/minecraft_demo/) 打開此頁面

## 作為擴充功能使用

可以在 MakeCode 中將此儲存庫新增為**擴充功能**。

* 開啟 [https://minecraft.makecode.com/](https://minecraft.makecode.com/)
* 按一下**新專案**
* 按一下工具齒輪選單下的**擴充功能**
* 搜索 **https://github.com/junming0106/minecraft_demo** 並匯出

## 編輯此專案

編輯 MakeCode 中的儲存庫。

* 開啟 [https://minecraft.makecode.com/](https://minecraft.makecode.com/)
* 按一下**匯入**，然後按一下**匯入 URL**
* 貼上 **https://github.com/junming0106/minecraft_demo** 並按一下匯入

#### 中繼資料 (用於搜索、渲染)

* for PXT/minecraft
<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
