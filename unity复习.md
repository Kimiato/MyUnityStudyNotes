《Unity2017从入门到精通》复习

# Chapter3 Unity编辑器

## 3.2 界面布局

- Scene View

  场景视图：设置游戏场景以及放置游戏对象，是构造游戏场景的地方

- Game View

  游戏视图：用于实时展示游戏运行的画面，处于播放模式的时候会被激活

- Hierarchy View

  层级视图：展示当前场景中的所有游戏对象

- Project View

  项目视图：显示整个工程项目中所有可用的资源

- Inspector View

  检视视图：查看当前所选择对象的属性和相关的一些信息

## 3.3 工具栏

---

### 3.3.1 Transform Tools（变换工具）

1. 手形工具（Q)

    可以在Scene视图中按鼠标左键平移整个场景

2. 移动工具（W)

    在Scene视图中选择某个对象之后，在该游戏对象上出现3个方向的箭头代表物体的三维坐标，通过拖动箭头可以改变游戏对象在某一个轴上的位置。

3. 旋转工具（E)

    可以在Scene视图中按任意角度旋转所选中的游戏对象。

4. 缩放工具（R)

    可以在Scene视图中缩放选中的游戏对象，蓝色方块代表沿Z轴缩放，红色X轴，绿色Y轴。中间的灰色方块可以将对象在3个坐标轴上进行统一的缩放。

5. 矩形工具（T)

    是允许用户查看和编辑2D或者3D游戏对象的矩形手柄。对于2D游戏对象，可以按住shift键进行等比例缩放。

6. 移动旋转缩放三合一工具（Y)

    包含W、E、R这三个快捷键代表的功能的整合工具。

在Scene视图中按住alt键配合鼠标左键可以以当前轴心点来旋转编辑视角，配合鼠标右键可以缩放编辑视角（拉进或拉远）

---

### 3.3.2 Transform Gizmo Tools（变换辅助工具）

- Pivot：该游戏对象（不包括子对象）的中心。

  Center：该游戏对象（包括子对象）的中心。

- Global：世界坐标

  Local：对象自身的坐标

---

### 3.3.3 Play（播放控制）

- 开始播放：command/Ctrl + P
- 暂停播放：shift + command/Ctrl + P
- 逐帧播放：option/alt + command/Ctrl + P

---

### 3.3.4 Layers（分层下拉列表）

控制游戏对象在Scene中的显示。下拉菜单中为显示状态的层级的物体（有眼睛图标）被显示在Scene视图中。

---

### 3.3.5 Layout（布局下拉列表）

用于切换，删除，保存的界面布局列表。

## 3.4 菜单栏

- File（文件）菜单主要包括场景和工程的创建、保存、输出等功能。
- Edit（编辑）菜单主要包括对场景一些列的编辑以及编辑器的设置等功能。

  Snap Setting 设置每次最小移动、缩放、旋转的单位
- Assets（资源）菜单提供游戏资源的管理功能，用于建立各种资源，导入和导出资源管理包。
- GameObject（游戏对象）菜单，用于创建游戏对象。
- Component（组件）菜单是用来添加到GameObject（游戏对象）上的一组相关属性，本质上每个组件都是一个类的实例。
- Window（窗口）菜单可以控制编辑器的页面布局，打开各种视图。
- Help（帮助）菜单包含unity相关的一些功能帮助，论坛、服务以及更新和其他的一些相关功能。

## 3.5 常用工作视图

---

### 3.5.1 Project

搜索过滤：t: 代表类型过滤，l: 代表标签过滤

---

### 3.5.2 Scene

按住鼠标的滚轮键，可以像使用快捷键Q一样移动场景。

- Flythrough：按住鼠标右键配合WAS/D键切换到该模式

  该模式下，以第一人称视角在Scene中飞行浏览，按住shift键可以加速移动

- Scene Gizmo工具：快速切换摄像机视角

  Top/Bottom/Back/Front

  可以鼠标单击该工具中间的方块或者下方文字，切换正交模式和透视模式

  - Isometric Mode 正交模式：

    无透视效果，物体不会随着距离的调整而缩小，**主要用于等距离场景效果以及GUI和2D游戏**

  - Perspective Mode 透视模式：

    模拟一个真实的三维空间，物体会随着距离的调整而缩放

  - 锁定视角：单击Scene Gizmo右上角的小锁，可以锁定，锁定后视角无法旋转，按住鼠标右键变成手形工具平移。

- Scene View Control Bar 场景视图控制栏

  - 可以改变摄像机查看场景的方式

    - 绘图模式
    - 2D/3D
    - Shaded模式
      控制对象的绘制方法，默认为Shaded，不会改变游戏的最终实现方式（仅作用于Scene）
    - 灯光开关
    - 切换天空球、雾效、光晕的显示与隐藏（P31）
    - Gizmos：同Game视图中的Gizmos，可以单击三角符号，实现显示或隐藏场景中用到的光源、声音、摄像机等对象的图标
    - 搜索栏：搜索物体的名称，会在Scene中带颜色突出显示，其他物体以灰色的方式显示，同时搜索结果也会在Hierarchy视图中显示出来

---

### 3.5.3 Game视图

显示游戏最终运行效果的预览窗口，无法编辑

Game View Control Bar：设置目标显示，分辨率，屏幕缩放等等

---

### 3.5.4 Inspector视图

展示选中游戏对象的一些信息和他带有的组件，常用的组件显示如下

- Transform

  可以修改游戏对象的Position，Rotation，Scale。该组件是游戏对象的基础组件，每一个游戏对象都有这个组件。

- Mesh Filter

  网格过滤器，用于从对象中获取网格信息，并将网格信息传递到网格渲染器。

- Mesh Render

  网格渲染器，从网格过滤器中获得几何形状，根据游戏对象的Transform组件中定义的信息还有光照进行渲染。

- Rigidbody

  刚体组件，可以使得物体能够感受力的作用，具有物理特性。

- Materials

  设置游戏对象的 Shader，颜色，贴图等等

---

### 3.5.5 Hierarchy层级视图

- 为游戏对象建立Parenting关系
- 让用户对大量对象的移动和编辑操作更加精确和方便
- 任何游戏对象可以拥有多个子对象，但是只能拥有一个父对象
- 对父对象进行的操作会影响到他所有的子对象，即子对象会继承父对象的数据，但是子对象可以进行独立的编辑操作。

---

### 3.5.6 Console控制台视图

在Console控制台视图中可以双击错误信息，即可打开代码编辑器自动定位有问题的脚本代码位置。


# Chapter4 游戏对象、组件和Prefabs

## 4.1 创建游戏对象和组件

1. 菜单栏 GameObject -> 3D Object -> Cube/Sphere
2. 创建完成的对象会在Hierarchy栏中显示，被称为游戏对象
3. 选中Cube游戏对象，可以看到他的4个组件
   - Transform
   - Cube(Mesh Filter)
   - Box Collider
   - Mesh Render
4. 给游戏对象添加组件
   - 选中要添加组件的游戏对象
   - 点击菜单栏中的component，弹出组件列表选中要添加的组件即可
     Hierarchy -> GameObject -> Component -> Physics -> Rigidbody

## 4.2 常用游戏对象

重命名物体的几种方式：

  - 在Hierarchy中选中物体后，再次单击
  - 在Hierarchy中选中物体后，按下F2（mac按下回车键）
  - 在Hierarchy中选中物体后，鼠标右键点击后选择Rename

---

### 4.2.2 Camera相机

可以在场景中拥有无数相机，可以为其设置任意顺序，在屏幕上的任何位置，或者仅仅在屏幕的某些部分进行渲染

参数列表：
- Depth Buffer：

  一个辅助的内存区域，大小与ColorBuffer相同，为图像的每个像素提供额外的深度信息，用于深度测试，对用户来说不可见。

  相机会将实时计算出来深度先缓存在一个表中，保留该值代表相机会先将实时计算的Depth Buffer在第一帧时存在表中，然后下一帧再读取表中的DepthBuffer，而不是相机实时计算出来的Buffer。这样后面的相机如果也有DepthBuffer，就会覆盖前一台相机的DepthBuffer，这个参数会影响到Clipping planes。

- ColorBuffer：

  图像输出的内存区域，GPU**把最后处理的颜色**写入这个区域，对应输出设备的像素点，向用户展示最终的显示效果，用户可见。

  相机会将实时计算出来的ColorBuffer在第一帧先存入表中，然后下一帧在读取表，这样后面的相机如果也有ColorBuffer就会覆盖掉前一个相机的ColorBuffer值。这里同DepthBuffer。

- Clear Flags：

  决定是否清除前面全部相机的ColorBuffer和DepthBuffer

  - Solid Color：

    清空前面全部相机的DepthBuffer和ColorBuffer，使用Background属性的颜色代替

  - Skybox：

    清空前面全部相机的DepthBuffer和ColorBuffer，使用天空盒代替

  - Depth Only：

    清空前面全部相机的DepthBuffer和ColorBuffer

  - Don't Care：

    不清空前面全部相机的DepthBuffer和ColorBuffer

- BackGround：

  当Clear Flag不是Skybox时，相机渲染的背景色

- Culling Mask：

  用于进行可选择性的渲染视图Scene，当GameObject的layerMask和cullingMask为0时，这个游戏对象在该相机下不可见

- Projection：

  - Perspective：以透视方式渲染
  - Orthographic：以正交模式渲染
  - Size：正交模式下，相机的视口大小
  - Field of View：透视模式下的相机视场角

- Clipping Planes：

  相机从开始到停止渲染的距离

  - Near：相机从开始到停止渲染的最小距离
  - Far：相机从开始到停止渲染的最大距离

- ViewPort Rect：

  相机渲染的位置和大小，在视口坐标中测量（0~1）

  - X:
  - Y:
  - W:
  - H:

- Depth：

  相机渲染的顺序，值大的会在值小的上面

- Rendering Path：

  定义相机渲染的方法

- Target Texture

  将相机渲染的画面输出到一个Render Texture纹理上

---

### 4.2.3 Light灯光

- Directional Light 方向光源

  可以被放置在无穷远处的位置，影响场景中的一切游戏对象，类似自然界中的日光，是最节约图形处理器资源的一种光源。

- Point Light 点光源

  类似电灯，从一个位置向四面八方发出光线，影响其范围内的所有对象。比较耗费图形处理器资源。

- Spot Light 聚光灯

  类似射灯的照明效果，处于锥形区域内的对象会受到光线的照射。比较耗费图像处理器资源。

- Area Light 区域光/面光源

  无法应用于实时光照，仅适用于光照贴图烘焙。

---

### 4.3.2 Mesh组件

Mesh组件有4种类型

- Mesh Filter

  网格过滤器。

- Text Mesh

  文本网格

- Mesh Renderer

  网格渲染器

- Skinned Mesh Renderer：

  蒙皮渲染器，用于呈现骨骼动画。

## 4.4 Prefabs预制体

可以理解为一个游戏对象及其组件的集合，目的是使游戏对象以及资源能够重复使用。


# Chapter5 构建3D场景

1. Terrain

   用于构建地形

   - 设置地形分辨率

     在Hierarchy视图中选中Terrain，然后在Terrain的Inspector视图中，点击Terrain下的齿轮设置按钮，修改Resolution下的Terrain Width(地形宽度)，Terrain Length(地形长度), Terrain Height(地形高度)。

   - 抬高地形，增加山脉，向下刷深度(shift+鼠标左键)

     喷涂地形高度时，可以通过点击喷涂选项下的Flatten按钮直接将地形统一抬高。

   - 添加纹理

     绘制地形的首层纹理，在Terrain的Inspector视图中，单击Terrain下的Paint Texture按钮，然后单击Edit Texture按钮，Add Texture，选择需要使用的纹理材质绘制。

   - 添加树木和植被

     在Terrain的Inspector视图中，单击Terrain下的Paint Trees按钮，将要添加的Tree材质添加进去，然后绘制。

     按住Shift键，然后单击场景中种好的树，可以将其移除。

     按住Ctrl键，在场景中可以移除范围内与选中类型相同的树。

     添加植被类似（P52），刷草时需要把视窗拉到刷草的地形上，距离太远的话花草不会展示在视窗上面，可以通过设置Detail Distance参数来调节。

   - Wind Setting for Grass

     - Speed：风吹过草的速度
     - Size：风吹过草地时的涟漪大小
     - Bending：草被风吹后的弯曲程度
     - Grass Tint：设置草对象的整体色调

   - Heightmap（高度图）

     导入或者导出Raw格式的地形高度图

   - Lighting（全局光照）P56

2. 光源与阴影

   - Mode

     - realtime

       每一帧实时计算照明（运行时计算），可以根据玩家动作或者场景中发生的事件变化而变化。

     - mixed

       可在运行时更改transform和视觉效果（照亮静态环境），运行时计算。

     - baked

       不在运行时计算，主要用于增加黑暗区域的亮度而无需调整场景中的照明。

       在动态对象上不能发出镜面照明，不能随着玩家动作和场景中的事件变化而变化，即是说没有动态的光照响应。动态游戏对象无法再与其他动态游戏对象上投射阴影。

3. 第一人称控制器

   - 控制器的高度应该高于其放置处的地向高度，否则会陷入地面，并且一直向下掉落。
   - 播放后通过 W A S D 控制移动，且播放时图标会被隐藏，可以使用快捷键结束播放，按esc会显示鼠标。
   - 可以通过将controller组件中的mouse look下的lock cursor参数取消勾选的方式，实现在播放时显示鼠标的功能。

4. 添加天空盒

   Window -> Lighting -> Settings，然后在打开的Lighting视图的Scene选项卡中，在Skybox Material选择需要使用的天空盒材质。

5. 添加音效

   - 添加BGM

     将bgm音频文件拖入Hierarchy视图中，然后在该bgm对象的Inspector视图中，勾选Loop。

   - 添加音效

     将对应的音频文件拖入Hierarchy视图中，然后在该对象的Inspector视图中，将Loop勾选，然后把Spatial Blend设置为1(这使得声音变成空间3D混合)，Volume Rolloff(音量衰减)设置为Linear Rolloff(线性衰减)，Max Distance能够覆盖掉需要的区域即可。


# Chapter8 3D数学基础

## 8.1 3D坐标系

unity中使用的是左手坐标系，其中 $x$ 轴代表水平方向，$y$ 轴竖直方向，$z$ 轴代表深度，即垂直纸面向里的方向。

unity中的游戏对象的坐标信息是放在一对括号中的，依次按照 $x、y、z$ 轴顺序的格式来写。

---

### 8.1.1 全局坐标系

在Scene中创建的物体，均以Global坐标系确定位置。

---

### 8.1.2 局部坐标系

- 每个物体都有独立的物体坐标系，随物体进行移动或者旋转
- 父子物体的坐标系相关联，子物体会以父物体的某一坐标点为自身的坐标原点

即是说，存在父物体时，position显示局部坐标系，无父物体时，position显示全局坐标。

---

### 8.1.3 相机坐标系

根据观察位置和方向建立的坐标系，方便判断物体是否存在于该相机的视野中，以及判断物体的先后遮挡顺序。

---

### 8.1.4 屏幕坐标系

建立在屏幕上的二维坐标系，描述像素在屏幕上的位置。原点位置 $(0, 0)$ 在屏幕的左下角，最大坐标在屏幕的右上角

## 8.2 向量

用于描述具有大小和方向两个属性的物理量，如物体运动的速度、加速度、摄像机的观察方向，刚体受到的力等等都是向量。

在数学中，既有大小又有方向的量就是向量。在几何中，向量可以用一段有方向的线段来表示。

---

### 8.2.1 向量的运算

- 加减
- 数乘

  向量与一个标量相乘称为数乘。数乘可以对向量的长度进行缩放，如果标量>0，向量进行数乘运算后的方向不变；若<0，反向。

- 点乘

  两个向量点乘得到一个标量。数值等于两个向量长度相乘后再乘以二者夹角的余弦值。

  $a · b = |a| * |b| * cosθ$

- 叉乘

  两个向量的叉乘得到一个新的向量。新向量垂直于原来的两个向量，并且长度等于原来向量长度相乘后再乘夹角的正弦值。

---

### 8.2.2 Vector3类

- 计算两个向量之间的距离

  `Vector3.Distance(obj1.position, obj2.position)`

- 使物体缓动到新的位置

  `Vector3.Lerp(obj1.position, target.position)`

## 8.3 矩阵

1. 平移

   平移矩阵
   $$
    Tp=\left[
    \begin{matrix}
      1 & 0 & 0 & 0 \\
      0 & 1 & 0 & 0 \\
      0 & 0 & 1 & 0 \\
      Px & Py & Pz &1 \\
      \end{matrix}
      \right]
   $$

   与 $v$ 相乘后

   $vT = (Vx + Px, Vy + Py, Vz + Pz, 1)$

   即实现 $v$ 沿 $v$ 方向平移 $(Px, Py, Pz)$ 距离'

2. 旋转

   旋转矩阵
   $$
    X(\theta)=\left[
    \begin{matrix}
      1 & 0 & 0 & 0 \\
      0 & cos\theta & sin\theta & 0 \\
      0 & -sin\theta & cos\theta & 0 \\
      0 & 0 & 0 &1 \\
      \end{matrix}
      \right]
   $$

   $X(\theta)$ 与 $v$ 相乘，可以使得向量 $v$ 沿 $x$ 轴旋转 $\theta$ 角。

3. 缩放

   缩放矩阵
   $$
    S(q)=\left[
    \begin{matrix}
      qx & 0 & 0 & 0 \\
      0 & qy & 0 & 0 \\
      0 & 0 & qz & 0 \\
      0 & 0 & 0 &1 \\
      \end{matrix}
      \right]
   $$

   $S(q)$ 与 $v$ 相乘，可以使 $v$ 在 $x, y ,z$ 的分量分别缩放 $qx, qy, qz$ 倍。

4. 组合

   现在有向量 $v$, 平移举证 $T$, 旋转矩阵 $R$, 缩放矩阵 $S$, 另有组合矩阵 $M=SRT$, 则有:

   $vSRT=vM$

   向量 $v$ 乘以矩阵 $M$ 相当于依次对 $v$ 进行缩放、旋转和平移。

## 8.4 齐次坐标

在3D数学中，齐次坐标就是吧三维向量 $(x, y ,z)$ 用四维向量 $(wx, wy, wz, w)$ 来表示。

引入齐次坐标的目的

- 更好的区分向量和点

  坐标点: $(x, y, z, 1)$

  向量: $(x, y, z, 0)$

- 统一用矩阵乘法表示平移、旋转、缩放变换

  如果用3x3矩阵，矩阵乘法只能表示旋转变换和缩放变换，无法表示其次变换。

- 当分量 $w=0$ 时可以表示无穷远处的点。

## 8.5 四元数

四元数包含一个标量分量和一个三维向量分量，四元数 $Q$ 可以记作: $Q=[w, (x, y, z)]$

用四元数表示对于三维空间内旋转轴为 $n$, 旋转角度为 $\alpha$ 的旋转：

$$
w = cos(\alpha/2)\\
x = sin(\alpha/2)cos(\beta x)\\
y = sin(\alpha/2)cos(\beta y)\\
z = sin(\alpha/2)cos(\beta z)\\
$$

其中 $cos(\beta x)、cos(\beta y)、cos(\beta z)$ 分别为旋转轴的 $x, y, z$ 分量。

使物体一直朝向 target 目标

```
Vector3 relativePos = target.position - transform.position;
transform.rotation = Quaternion.LookRotation(relativePos);
```

## 8.6 坐标变换原理

---

### 8.6.1 世界坐标与局部坐标的变换

- 局部坐标->全局坐标

  `Transform.TransformPoint`

- 全局坐标->局部坐标

  `Transform.InverseTransformPoint`

- 向量的全局坐标和局部坐标转换

  `Transform.TransformDirection`

  `Transform.InverseTransformDirection`

---

### 8.6.2 世界坐标与屏幕坐标转换

(以相机为媒介)

- 世界坐标->屏幕坐标

  `screenPos = Camera.main.WorldToScreenPoint(transform.position);`

- 屏幕坐标->世界坐标

  `Vector3 worldPos = Camera.main.ScreenToWorldPoint(mousePos);`


# Chapter10 信息输入管理

## 10.1 Input Manager

Input类的部分成员变量

| 变量名 | 作用 |
| :--- | :--- |
| anyKey | 是否有按住 |
| anyKeyDown | 是否有按下 |
| compass | 罗盘 |
| backButtonLeavesApp | 是否按下退出按钮退出APP |
| compensateSensors | 是否需要根据屏幕方向补偿感应器 |
| compositionCursorPos | 当前IME组合字符串的光标位置 |
| gyro | 返回默认的陀螺仪 |

---

Input类的部分成员函数

| 函数名 | 作用 |
| :--- | :--- |
| GetAccelerationEvent | 返回上一帧期间发生的特定加速度测量 |
| GetAxis | 根据名称得到虚拟输入轴的值 |
| GetAxisRaw | 根据名称得到虚拟坐标轴的未使用平滑过滤的值 |
| GetButton | 指定名称按钮**按住**时，返回true |
| GetButtonDown | 指定名称按钮**按下**时，返回true |
| GetButtonUp | 指定名称按钮**松开**时，返回true |
| GetTouch | 返回指定的触摸数据对象（不临时分配变量） |
| GetJoystickNames | 返回当前连接的所有摇杆的名称数组 |

---

类似的几个Input类的成员函数

- GetKey
- GetKeyDown
- GetKeyUp
+ GetMouseButton
+ GetMouseButtonDown
+ GetMouseButtonUp

## 10.2 鼠标输入

|  |  |
| :--- | :--- |
| mousePosition | 获取当前鼠标指针位置的像素位置(只读) |
| GetMouseButtonDown | 鼠标按键按下的第一帧返回true |
| GetMouseButton | 鼠标按键按住期间一直返回true |
| GetMouseButtonUp | 鼠标按键松开的第一帧返回true |
| GetAxis("Mouse X") | 得到第一帧内鼠标在水平方向的移动距离 |
| GetAxis("Mouse Y") | 得到第一帧内鼠标在垂直方向的移动距离 |

`GetMouseButtonDown`、`GetMouseButton`、`GetMouseButtonUp`需要传入参数来指定判断哪个鼠标按键：**0对应左键，1对应右键，2对应中键**

## 10.3 键盘输入

键盘输入有些需要配合KeyCode编码来使用

一些例子

`GetKey("up")`

`GetKey(KeyCode.DownArrow)`

`GetKeyDown(KeyCode.Space)`

`GetKeyUp(KeyCode.Space)`

`GetAxis("Horizontal")` 和 `GetAxis("Vertical")`: 用方向键或者W、A、S、D键来模拟-1到1的平滑输入。

## 10.6 自定义输入

创建虚拟按键: Edit -> ProjectSetting -> Input

virtual button 是输入轴的一种特殊情况


# Chapter11 物理系统

## 11.1 概述

unity中有两个独立的物理引擎，一个3D物理引擎，一个2D物理引擎。俩物理引擎之间的概念是相同的（除了额外的3D维度），但是它们使用的是不同的组件来实现的。

---

## 11.2 物理系统相关组件

---

### 11.2.1 刚体组件

Rigidbody(刚体)组件，包括Rigidbody和Rigidbody 2D


作用:
- 使游戏对象在物理系统的控制下进行运动
- 接受外力和扭矩力 => 保证游戏对象像在真实世界中移动
- 使游戏对象受到重力印象
- 作用力：通过NVIDIA物理与其他游戏对象的互动的运算，都需要添加Rigidbody


如何添加Rigidbody
- 方法一：

  选中待添加刚体组件的对象

  点击 Component -> physics -> Rigidbody

- 方法二:

  选中待添加刚体组件的对象

  在Inspector中，单击下方Add Component，搜索Rigidbody添加


Rigidbody的属性

- Mass 质量

  同一Scene中，不同obj的质量之比不要超过100倍

- Drag 阻力

  obj游戏对象进行受力运动时受到的空气阻力

- Angular Drag 角阻力

  当游戏对象受到扭矩力旋转时受到的控制阻力

- Use Gravity 使用重力

- Is Kinematic 是否开启动力学

  开启后，不再受到物理引擎的影响，只能通过Transform来操作，适用于模拟平台的移动或者带有铰链关节链接刚体的动画。

- Interpolate 插值

  用于控制刚体运动的抖动情况

  - None 无
  - Interpolate 内插值，基于**前一帧**的Transform来平滑此次的Transform
  - Extrapolate 外插值，基于**下一帧**的Transform来平滑此次的Transform

- Collision Detection 碰撞检测

  避免高速运动的物体穿过其他的游戏对象而且未发生碰撞情况。

  - Discrete

    离散碰撞检测。

    游戏对象与场景中其他的所有物体进行碰撞检测，默认值。

  - Continuous

    连续碰撞检测。检测游戏对象obj与动态碰撞体的碰撞。

    可检测obj与网格碰撞体(没有Rigidbody)的碰撞。适用于要采用连续动态碰撞检测的物件。

    特点: 对物理性能有很大影响，如果不需要对快速运动的游戏对象进行碰撞检测，就使用Discrete。

  - Continuous Dynamic

    连续动态碰撞检测

    主要用于检测obj与**采用连续动态碰撞或连续碰撞的对象的碰撞**

    也可以用于检测没有Rigidbody的静态网格碰撞体

    可以用于检测快速运动的游戏对象

- Constraints 约束

  - Freeze Position 冻结位置，使刚体在这个勾选轴方向上的**移动**无效。

  - Freeze Rotation 冻结某个轴的旋转，是刚体在勾选轴方向上的**旋转**无效
---

### 11.2.2 角色控制器

Character Controller(角色控制器)主要用与对第一人称或者第三人称游戏主角的控制，并不使用刚体的物理效果。

Character Controller组件属性面板

- Slope Limit

  坡度限制。游戏对象只能爬上小于或者等于该参数值的斜坡。

- Step Offset

  台阶高度。游戏对象只能迈上小于或等于该值高度的台阶。

- Skin Width

  皮肤厚度。该参数决定了两个碰撞体可以相互渗入的深度。

  较大 -> 产生抖动现象

  较小 -> 导致被控对象obj被卡住

  合理值: Radius的10%

- Min Move Distance

  最小移动距离。如果被控对象的移动距离小于该值，则游戏对象不会移动。

  目的是为了防止抖动。大多数情况下把该值设为0。

- Center

  决定胶囊碰撞体与所控制obj的游戏对象的相对位置。不影响所控制obj的中心坐标。

- Radius

  Capsule碰撞体的半径。

- Height

  Capsule碰撞体的高度。

注意：
- 角色控制器**不会对施加给它的作用力作出反应，也不会作用于其他刚体**
- 可以在`OnControllerColliderHit()`函数中，为与其碰撞的对象施加上一个作用力
- 如果想要让Character Controller 受力作用，可以使用刚体替代

---

### 11.2.3 碰撞体组件

作用

- 要与刚体一起添加到游戏对象上，才能发生碰撞
- 在物理引擎中，没有添加碰撞体的两个物体会彼此相互穿过

碰撞体类型

1. Box Collider 盒碰撞体

   - Edit Collider 编辑碰撞体。点击后可以在Scene编辑碰撞体形状
   - Is Trigger 触发器。勾选后，该碰撞体可以用于触发事件，**且将被物理引擎忽略**
   - Material 材质。采用不同材质的碰撞体和其他对象交互的形式不同。
   - Center 中心。碰撞体在**局部坐标**中的位置
   - Size 大小。碰撞体在 x, y, z 方向上的大小

2. Sphere Collider 球形碰撞体

   - Edit Collider
   - Is Trigger
   - Material
   - Center
   - Radius 半径

3. Capsule Collider 胶囊碰撞体

   unity角色控制器中通常内嵌了Capsule Collider

   - Edit Collider
   - Is Trigger
   - Material
   - Center
   - Radius
   - Height 高度。控制胶囊体中圆柱的高度。
   - Direction 方向。在对象的局部坐标中胶囊的纵向所对应的坐标轴。

4. Mesh Collider 网格碰撞体

   与基础碰撞体相比，Mesh Collider更加精细，也更加占用资源。
   只有在开启了Convex参数的网格碰撞体才能与其他的网格碰撞体发生碰撞。

   - Convex 凸起。
   - Is Trigger
   - Material
   - Mesh 网格

   Mesh Collider根据所附加对象的Transform来设定碰撞体的位置和大小比例。使Collider的形状与GameObject的可见网格形状完全相同。正因为如此，所以开销比较大，尽量少用。

   **碰撞网格**：碰撞网格使用了背部消隐的方式。如果一个obj与一个背部消隐的Mesh在是视觉上发生碰状态，他们并不会在物理上碰撞。

   网格碰撞体限制：
     - 通常两个Mesh Collider之间不会碰撞。
     - Mesh Collider可以与基本的碰撞体发生碰撞。
     - 只有网格碰撞的Mesh中三角形数量少于255时，Convex才能生效。

5. Wheel Collider 车轮碰撞体

   针对地面车辆，内置碰撞检测，车轮物理系统，有滑胎摩擦的参考体

   - Mass 质量

   - Radius 半径

   - Wheel Damping Rate 车轮阻尼率

   - Suspension Distance 悬挂距离

     用于设置车轮碰撞体悬挂的最大伸长距离，按照**局部坐标**计算。

     悬挂总是通过其局部坐标的y轴进行延伸。

   - Force APP Point Distance 力作用点距离。

     预计为从车轮静止位置沿悬架行进方向的距离。更好的车辆将力应用于略低于车辆质心的位置。

   - Center 中心。

     设置车轮碰撞体在对象局部坐标中的位置。

   - Suspension Spring 悬挂弹簧。

     设置车轮碰撞体通过添加弹簧和阻尼外力使得悬挂达到目标位置

     - Spring 弹簧。弹簧力度越大，悬挂达到目标位置的速度也越快。
     - Damper 阻尼器。数值越大，悬挂弹簧移动速度越慢。
     - Target Position 目标位置。悬挂沿着方向上静止时的距离。值为0，完全伸展状态；值为1，完全压缩状态。默认0.

   - Forward Friction 前向摩擦力。

     - Extremum Slip 滑动极值
     - Extremum Value 极限值
     - Asymptote Slip 滑动渐进值
     - Asymptote Value 渐进值
     - Stiffness 刚性因子。为极限值与渐进值的乘数(默认为1，表示刚度变化的摩擦程度。设置为0禁用所有的车轮摩擦。通常在运行时脚本修改来模拟各种地面材料)

   - Side Friction 侧向摩擦力

     - Extremum Slip
     - Extremum Value
     - Asymptote Slip
     - Asymptote Value
     - Stiffness

6. Terrain Collider 地形碰撞器

   - Material 材质
   - Terrain Data 地形数据
   - **Enable Tree Colliders** 开启树的碰撞体

---

### 11.2.4 物理材质

添加方式

Assets -> Create -> Physics Material。然后将物理材质从Project项目视图拖放到场景中的碰撞体上即可。

属性列表

- Dynamic Friction 动摩擦系数 通常值 $\mu\in[0, 1]$
- Static Friction 静摩擦系数 通常值 $[0, 1]$
- Bounciness 弹力系数 0不会反弹，1会反弹且无能量损失
- Friction Combine 两个碰撞体摩擦的组合方式
  - Average 平均值
  - Minimum 最小值
  - Maximum 最大值
  - Multiply 乘积
- Bounce Combine 两个碰撞体弹性的组合方式，具体方式类型同上摩擦的组合方式

注意：**组合方式的优先级**: Average < Minimum < Multiply < Maximum

---

### 11.2.5 布料组件

布料组件可以模拟类似布料的行为状态。

包括：
- Skinned Mesh Renderer 蒙皮网格渲染器
- Cloth

其中 Cloth 和 Skinned Mesh Renderer 要协同工作。即是说 Cloth 只适用于蒙皮网络。

将 Cloth 组件添加到非蒙皮网格时，unity会自动移除非蒙皮网格渲染器并添加蒙皮网格。

Skinned Mesh Renderer 参数：

- Quality 品质。在蒙皮时每个顶点使用的骨骼的最大数量，设置为自动时，以使用质量设置的混合权重值。

- Update When Offscreen 蒙皮网格更新。启用后，即使所有Camera都不可见，Skinned Mesh也会更新。禁用后，当GameObject不在屏幕上时，动画本身会停止运行。

- Mesh 网格。

- Root Bone 骨骼根节点。

- Bounds 限制范围

  - Center 网格中心位置
  - Extents 网格的范围

- Lighting 光线参数 P175

  - Light Probes 基于光照探头的内插模式

  - Reflection Probes 如果启用且反射探头出现在场景中，反射纹理会从这个游戏对象和构建着色器设置的变量中获取到。

  - Anchor Override 用于设置光照探头或者反射探头系统时内插文职的Transform

  - Cast Shadows 投射阴影

    off 关闭投射阴影

    on 开启透射阴影

    Two Sided 开启双面阴影

    Shadows Only 只投射阴影

  - Receive Shadow 接受阴影

  - Motion Vector 用于设置运动矢量的渲染模式

  - Material 材质列表

  - Dynamic Occluded 动态遮挡

Cloth 参数 P175

- Stretching Stiffness 拉伸刚度。用于设置抗拉伸程度，值越大越不容易拉伸。

- Bending Stiffness 弯曲强度。用于设置抗弯曲程度，值越大越不容易弯曲。

  ...

特点
  布料不会对Scene中的碰撞体做出反应，也不会是施加力量，可以为布料添加碰撞体来模拟反应，但是始终无法施加力，若不添加，世界与布料互不识别。

---

### 11.2.6 关节组件

1. Hinge Joint 铰链关节

由两个刚体组成，关节对刚体进行约束， 适用于门，模型链，钟摆

属性

| 属性名 | 作用 |
| :--- | :--- |
| Edit Joint Angular Limit | 编辑关节角度的限制 |
| Connected Body | 连接刚体（为关节指定Body），不指定则连接世界 |
| Anchor | 锚点（位置应用于局部坐标系） |
| Axis | 轴，定义刚体摆动方向（局部坐标） |
| Auto Config Connected Anchor | 自动连接锚点，默认开启 |
| Connected Anchor | 链接锚点，Auto开启时默认开启，Auto关闭时手动连接 |
| Use Spring | 使用弹簧->使刚体与连接主体形成特定角度 |
| Spring | 弹簧 Spring 弹簧力, Damper 阻尼, Target Position 目标角度 |
| Use Motor | 使用马达，使对象rotate  Target Velocity 目标速度, Force 作用力, Free Spin 自由转动 |
| Use Limits | 使用限制->勾选后铰链角度将被限定区间 |
| Limits | Min/Max 铰链能达到的最小/大角度, Min/Max Bounce 最小/大反弹(铰链对象接触到最小值的反弹值), Max Bounce |
| Break Force | 断开力 |
| Break Torque | 断开扭矩 |
| Enable Collision | 激活碰撞(关节间) |
| Enable Preprocessing | 启用预处理(禁用有助于稳定无法执行的配置) |
| Mass Scale | 质量缩放值 |
| Connected Mass Scale | 连接刚体的质量缩放值 |

2. Fixed Joint 固定关节

使用固定关节的对象自身要有一个刚体。适用于某些obj要暂时或者永久的连接在一起。

特点：不需要通过脚本来修改层级结构就能实现

3. Spring Joint 弹簧关节

参数：
- Spring 弹簧强度
- Damper 阻尼
- Min Distance 弹簧启用的最小距离
- Max Distance 弹簧启用的最大距离

其余参数同Hinge Joint

4. Character Joint 角色关节

参数P182：
- Swing Axis 摆动轴，设置角色关节摆动轴
- Twist Limit Spring 弹簧的扭曲限制: Spring/Damper
- Low Twist Limit
  - Limit 扭曲下限
  - Bounciness 扭曲下限反弹值
  - Contact Distance 为了避免抖动限制的接触距离

5. 可配置关节

---

### 11.2.7 力场组件

为刚体快速添加恒定作用力，适用于火箭发射这类，游戏对象在起初时没有很大的初速度，但不断加速的


## 11.3 可视化物理调试

允许用户快速检查 Scene中的几何碰撞体，提供了ojbs应该和不应该相撞的可视化情况

window -> Physics Debugger


# Chapter12 粒子系统

## 12.1 什么是粒子系统

- 粒子是小的、简单的图像或网格
- 粒子系统可以显示和移动大量粒子

1. 系统动力学

   每个粒子都有预定的寿命，可在球，半球，锥，立方体或任意网格形状的空间内随机发射粒子，显示粒子直到其寿命结束，此时从系统中被排放。

2. 粒子动力学

   发射和寿命会影响系统的整体行为，每个粒子的颜色，大小，旋转方式都可以随时间和运动变化，通常在Scene中生成大量2D图像来模拟流体实体

## 12.2 在unity中使用粒子系统

方法一: 直接创建粒子对象

GameObject -> Effects -> Particle System

方法二: 在GameObject中添加粒子系统组件

Component -> Effects -> Particle System

动画绑定: 动画系统可以访问所有粒子系统属性，即是说，可以将它们设为关键帧，并在动画中控制它们。

## 12.4 参数详解

1. Main 主模块

   固有module，定义粒子初始化时的持续时间，大小，发射速度，循环方式等。

2. Emission 发射模块

   控制粒子的放射速度，可以实现在某个特定时间内生成大量粒子的效果，有利于模拟爆炸等情况

3. Shape 形状模块

   定义粒子从中发射的形状(体积or表面积)，以及起始速度方向

   参数：
    - Shape

      粒子发射器的形状，shape不同，Particle的初始速度方向不同，Sphere，Hemisphere有相同参数属性

    - Cone 锥形发射器
    - Donut 圆环发射器
    - Box 方块发射器
    - Circle 圆圈发射器
    - Edge 边沿发射器

4. Velocity over Lifetime

   - 控制生命周期内每个粒子的速度
   - 对行为复杂的粒子效果明显
   - 对简单视觉行为的粒子(如烟雾)以及与物理世界几乎没有互动的粒子作用不明显

   参数:
   - x, y, z => x, y, z轴向的速度
   - Space => 所选 x, y, z 轴是local还是world
   - Speed Modifier => 沿例子当前行进方向对粒子的速度应用乘数

5. Limited Velocity over Lifetime

   控制生命周期内的限制速度以及衰减速度，可以模拟类似拖拽的效果
   参数:
   - Dampen 超过限制$v$时，粒子$v$降低的部分
   - Drag 应用线性牵引于粒子速度
     - Multiply by Size 启用时，粒子**大小**越大，受阻力系统越大
     - Multiply by Velocity 启用时，粒子**速度**越大，受阻力系数越大

6. inherit Velocity

   控制粒子随时间推移，速度对于父对象运动的反应
   Mode:
    1. Current 发射器当前速度应用于每一帧上所有粒子，发射器$v$越小，所有粒子$v$越小
    2. Initial 每个粒子诞生时，会被发射器施加一次速度，粒子诞生后，发射器速度任何变化都不会影响粒子
    3. Multiplier 粒子按照指定比例继承发射器速度

7. Force over Lifetime

   控制粒子加速度
   参数:
   - x, y, z => x, y, z轴向的速度
   - Space => 所选 x, y, z 轴是local还是world
   - Randomize => 使用Tow Constant或者Tow Curves模式时，随机化会产生更不稳定的运动

8. Color over Lifetime

   设置粒子在生命周期内的颜色和透明度的变化

   参数:
   - Color => 粒子在其整个生命周期中的颜色梯度(起->止)

9. Color by Speed

   参数:
   - Color 在速度范围内定义的粒子的颜色梯度
   - Speed Range 颜色渐变映射到速度范围的min&max

10. Size over Lifetime

    参数:
    - Separate Axes 是否在每个轴上独立控制粒子大小
    - Size 定义每个粒子的大小在其生命周期变化的曲线

11. Size by Speed

    参数
    - Separate Axes
    - Size
    - Speed Range

12. Rotation over Lifetime

    参数
    - Separate Axes
    - Angular Velocity 旋转速度(每秒)

13. Rotation by Speed

    参数
    - Separate Axes
    - Angular Velocity
    - Speed Range

14. External Force 外部力量模块

    用于设置风区对粒子的影响

15. Noise

    用于给粒子系统添加湍流效果

    - 高频噪声可以用来模拟火焰余烬
    - 低频噪声可以模拟烟雾效应

    参数
    - Separate Axis
    - Strength
    - Frequency
    - Scroll Speed
    - Damping
    - Octaves 振幅
    - Octave Multiplier
    - Octave Scale
    - Quality
    - Remap
    - Remap Curve 描述最终噪声如何转换
    - Position Amount
    - Rotation Amount
    - Size Amount

16. Collision

    控制粒子与游戏对象的碰撞

    参数:
    - planes 一个可以扩展的Transform对象，定义碰撞的平面
    - Visualization 可视化=>碰撞平面显示是框线风格还是固体平面
    - Scale Plane 设置可视化平面大小
    - Dampen 碰撞后的粒子速度损失
    - Bounce 碰撞反弹后的粒子速度
    - Lifetime Loss 碰撞后的粒子生命周期的损失
    - Min Kill Speed 粒子在小于该速度时，碰撞后销毁
    - Max Kill Speed ......大于......
    - Radius Scale 粒子碰撞半径的大小
    - Send Collision Messages 激活后，粒子发射碰撞时调用
    - Visualize Bounds 是否显示每个粒子碰撞边界的线框形状

    world选项 P206

17. Triggers

    控制粒子系统在场景中的一个或者多个触发器。发生触发时调用回调函数

    - Colliders 与粒子相撞的碰撞器列表
    - Inside 粒子在触发器内(Ignore/Kill/Callback)
    - Outside 粒子在触发器外
    - Radius Size 设置粒子碰撞体的大小
    - Visualize Bounds 是否显示每个粒子碰撞边界的线框形状

18. Sub Emitters 子发射器

    - Birth 粒子产生时发生的子粒子
    - Collision 粒子碰撞时发射的子粒子
    - Death 粒子死亡时发射的子粒子

19. Texture Sheet Animation 纹理动画模块

    可以把纹理作为一个独立的子图像网格，用于播放帧动画

20. Lights 灯光模块

    给粒子添加实时灯光

21. Trail 拖尾模块

    给粒子运动路径添加拖尾效果

22. Custom Data 自定义数据

    给粒子附加自定义数据格式

23. Render 渲染模块

    用于设置粒子系统渲染相关属性


# Chapter13 动画系统

## 13.1概述

特点:
- 支持向 unity 中导入动画，或者直接在 unity 中创建动画
- 一个游戏动画可以应用子不同的⻆色模型
- 简化了流程，方便剪辑，转换和交互
- 可视化编辑工具
- 支持动画分层遮罩
- 不同身体部位使用不同逻辑

动画系统工作流:
- Unity 动画系统基于动画剪辑
- 动画片段可以来自于 3ds Max，Maya 等第三方工具
- 可以将动画片段组织成【动画制作器】+【控制器】的系统 类似于结构化流程图
- 动画控制器:
  用作“状态机“ 可跟踪当前播放的动画剪辑，以及动画剪辑改变或混合时的状态信息

Unity 动画系统人形⻆色处理:
- 支持运动捕捉，资源存储 或 第三方动画库
- 人形字符可以被映射到通用的内部模式

Unity 动画工作流主要阶段:
1. 资源的准备和导入
   由【美术】或【动画师】通过第三方工具完成

2. ⻆色的建立
   - 人形⻆色建立:

     Mecanim 通过扩展的图形操作界面和动画重定向功能，为人形模型提 供特殊的工作流，包括 Avatar 的创建和对肌肉定义的调节等

   - 一般⻆色建立:

    为处理任意的运动物体和四足动物设定的，动画重定向功能对此不适用

3. ⻆色的运动 包括创建动画片段及其相互间的交互作用，包括建立状态机和混合树，调整动画参数，以及通过代码控制动画等

## 13.2 Unity 动画相关组件

---

### 13.2.1 Animator 和 Animator Controller

1. Animator 动画组件

   Animator 视窗与 Scene 视窗同级，并排显示

   作用: 用于将动画分配给场景中的 GameObject。需要引用动画控制器来使用。

   引入动画控制器的原因: 定义要使用哪些动画片段，并控制 when & how to 在其间进行混合或转换。如果 GameObject 是具有 Avatar 定义的人形⻆色，则组件中也应该分配 Avatar 动画组件，动画曲线信息参数⻅ P214

2. Animator Controller 动画控制器

   **作用**: 允许用户为⻆色或其他动画游戏对象安排和维护一组动画。对其中使用的动画片段进行了引用, 并使用状态机管理各种动画状态和它们之间的转换，要使用动画剪辑时，需要用一个动画控制器来整合资源，所以即使只有一个动画剪辑，仍然需要将其放在动画控制器中。

   **状态机**: 可以认为是一种流程图，或者是简单的 Unity 程序内的视觉编程语言

   **创建方式**: Create -> Animator Controller。以上操作会创建一个 .controller 格式的资源

   **动画控制器的窗口内容**:  Layer 动画层组件; Parameters 事件参数组件;状态机自身的可视化窗口

3. Layer 动画层组件

   **作用**: 可以管理身体不同部位的复杂状态机。如，使用下半身层来管理 走动 / 跑动，上半身层来管理 投掷 / 射击

   **使用方式**: 可以从动画控制器左上⻆的图层小部件(Layers)中管理动画图层，单击图层菜单右侧的小⻮轮，可以显示该图层的设置

   **图层功能及如何使用**: 在每个图层上，用户都可以指定遮罩和混合类型。Override 意味着来自其他图层的信息将被忽略。Additive 意味着动画将被添加到之前的图层上。点击 Animator - Layers 视窗中的 + 按钮 可以添加新图层。

4. Parameters 参数组件

   在 Animator Controller 中定义的变量，可以从脚本中访问并分配值，脚本可以控制或影响状态机的流程

   默认参数可以在 Animator 窗口左下⻆的 Parameters 工具栏中设置

   **参数类型**: Float，Int， Bool， Trigger

5. 动画状态机

   一个⻆色拥有多个可以在游戏的不同状态下调用的不同动作是普遍的现象，使用脚本来控制这些动作是潜在的复杂工作。Mecanim 借用了状态机的概念来简单地控制和序列化⻆色动画

   **状态机**: 基本观点是，一个⻆色应该在任何给定的时刻，执行某些特定的动作。一般情况下，⻆色在进入下一个状态时应该有所限制，而不是跳到任意状态，将这些情况整合起来的东⻄就是状态机。状态和状态转移可以使用图形界面描述，在这个界面里，节点用来描述状态，而带箭头的线段表示状态转移

   Mecanim状态机：提供了一种可以预览某个独立⻆色的所有动画剪辑集合的方式

   状态机包括: 状态，状态转移，事件。大状态机中可以再设置小的子状态机

   - 动画状态

     动画状态机中内建的基本模块

     每个状态包含一个在该状态下⻆色能播放的独立动画序列。出发状态转移事件时，⻆色将会转移至动画序列指定的下一个状态。在复杂状态机中，预览独立的状态机中的某些部分可以提升效率。

     特殊功能: 用户可以使用静音和独奏功能(Mute，Solo)。静音:转换将被禁用；独奏:相对于源自相同状态的其他转换会被弃用。在过渡检查器或状态检查器(更推荐)中设置 Mute 和 Solo，在视图中，设置为 Solo的状态转换为绿色箭头，Mute为红色箭头。**当一个 Solo 被勾选，则该状态的其余转换将被 Mute，如果 Solo 和 Mute 都被勾选，则 Mute 优先级更高。**

     创建新状态: 在动画控制器窗口的空白区域单击鼠标右键，选择 Create State -> Empty 来创建一个新的状态。向动作控制窗口拖拽一个新的动画，以此创建一个包含该动画的动画状态(用户只能拖拽 Mecanim 系统动画)。

     一些技巧: 状态机首次被激活时，会自动跳转至橘⻩色的默认状态，用户可以根据需求自行更改默认状态。

     修改默认状态:  右键某个状态，在弹出菜单中选择 Set As Default State。

     快捷键: Alt + 鼠标左键拖动，可以移动状态机视图，滚动鼠标滚轮，可以缩放状态机视图。

     注意，动画状态也可以包含一个动画混合树，参数⻅ P218

   - Any State 任意状态

     一个一直存在的特殊状态

     作用: 为了保证在任意状态下可以转移至某个当前正处于的特殊状态而准备的

     特点: 不能作为一个状态转移的重点

   - Entry 和 Exit 节点

     动画窗口的每个视窗都有一个 Entry 和 Exit 节点

     作用:
       - Entry: 在转换到当前状态机时使用, 可以根据预条件，设置倒不同的分支状态
       - Exit: 用于指示状态机应该退出

   - Animator Transition 动画过渡

     是状态机直接的连线

     作用: 帮助用户简化大型货复杂状态机, 允许用户在状态机逻辑上有更高的抽象级别

     如何添加/删除: 选中某个过渡的状态机，点击Make Transition -> 创建动画过渡方式。选中某条过渡线，按键盘 Delete键 -> 删除动画的过渡方式。

     当用户从一个动画状态跳转到另一个动画状态时，发生动画过渡。选中动画过渡线即可看到过渡动画的设置。

     参数:
     - Has Exit Time: 动画过渡是否有固定的退出时间
     - Exist Time: 动画过渡时，本状态退出的时间
     - Fixed Duration: 若勾选 Has Exit Time，以秒为单位进行转换, 为勾选 ... , 转换时间将被理解为源状态的归一化时间的一小部分
     - Transition Duration: 当前状态持续时间，或转换的持续时间, 在转换图中，可视化为两个蓝色标记之间的部分(P220 13-16)
     - Transition Offset: 在转换到的目标状态中，开始播放的时间偏移量, 例如 0.5 表示目标状态通过其时间线以原先50%的速度开始播放
     - Interruption Source: 使用它来控制这种转换可能被中断的情况
     - Ordered Interrupution: 确定当前转换是否可以独立于其顺序中的其他转换
     - Conditions: 设置何时触发该动画过渡

     转换条件和时间作用: 转换可以 0 到 多个 转换条件，为 0 时，Unity 只考虑退出时间,如果用户的转换至少有一个条件，则在触发转换钱必须满足条件。

     触发条件包括: Conditions 触发条件。一个条件参数: 可以用 Exit Time 为参数并声明一个表示为源状态标准的时间参数。如，0.95表示该状态转移会在原动画播放至(95%时触发)；一个条件谓词: 如果需要，使用浮点数作为参数时，可以使用小于 / 大于 的数；一个条件值: 如果需要，使用整数作为参数时，判断是否等于一个固定值。

     注意: 如果转换启用了 Has Exit Time 并且至少有一个条件, 则仅在状态退出时间后才会检查这些条件。

---

### 13.2.2 Animation 动画编辑器

Animation 窗口是 Unity 提供的，用来编辑物体动画的系统

1. 动画编辑

   打开编辑窗口: 选中游戏对象，点击 Window -> Animtion 打开动画编辑窗口

   **创建一个动画组件**：若选中的游戏对象没有动画，则在 Animation编辑窗口右侧有 Create 按钮，点击 Create 即可弹出创建动画窗口。设置完毕后，点击创建动画窗口的 Save 按钮即可保存一个动画文件，该动画文件保存到 Project 视图中，此时 Unity 还会创建一个与所选 GameObject 同名的 Animator Controller，将一个 Animator 组件添加到 GameObject中，并适当地连接资源。

   动画窗口属性: ⻅ P 221 13-18
   - 开启 / 关闭 动画录制
   - 播放 / 暂停 动画效果
   - 动画采样帧数 samples
   - 添加动画属性 add property
   - 动画关键帧 key ⻅ P 222 13-19
     - key 关键帧; event   动画事件
     - 添加 key 左侧视窗棱形按钮，右侧网格处 单击鼠标右键 -> 添加key
     - 添加 event 左侧视窗竖条形按钮，右侧网格上方空白处 单击鼠标右键

2. 动画设置

   打开动画文件: 在 Projects 面板中，找到已经录制好的动画片段, Assets中图标为播放键的文件,随后在属性面板里设置动画片段属性，并预览动画效果

   参数:
   - Loop Time 是否循环
     - Loop Pose 勾选后动画进行无缝循环
     - Cycle Offset 需要在不同的时间启用动画，则设置循环动画的周期偏移

   预览: 位于动画片段的属性面板右下⻆，即属性面板中参数下方的可视化窗口处

## 13.3 外部动画资源的准备和导入

---

### 13.3.1 获取人形网格模型

1. 人形网格模型

   为充分利用 Mecanim 的人形动画系统，以及动画重定向功能，需要一个觉有 ⻣骼绑定 和 蒙皮 的 人形网格模型

   创建一个人形网络模型的步骤:
   - 一般由一组多边形或三⻆形网格组成 创建模型的过程被称为建模(modeling)
   - 为控制⻆色运动，必须创建一个⻣骼关节层级(joint hierarchy), 该层级定义了网格内部的 ⻣骼结构 及其 相互运动关系,这个过程被称为⻣骼绑定(rigging)。
   - 人形网络模型必须与关节层级关联起来，即通过指定关节的动画来控制 特定网格的运动，这个过程被称为蒙皮(skinning)。

2. 如何获取模型

   在 Mecanim 系统中，有三种途径获取人形网格模型
   - 使用一个过程式的 人物建模 软件，如 Poser，Makehuman，或者 Mixamo。其中 Mixamo 可以同时进行 ⻣骼绑定 和 蒙皮操作。(Tip:在软件中应该尽量减少人形网格的面片数量->性能)
   - 在 Unity Asset Store 上购买适当的模型资源
   - 通过其他建模软件来创建全新的人形模型, 包括 3ds Max， Maya， Blender 等

3. 导出和验证模型

   Unity 引擎可以导入一系列常用的 3D 文件格式，推荐使用 FBX 2012

   FBX 2012 的特点: 导出的网格中可以包含 关节层级，法线，纹理，以及 动画信息(不包括蒙皮)，可以将网格模型重新导入建模软件，从而验证其正确性。可以直接导出不包含网格的动画信息

---

### 13.3.2 导入动画

可以导入的动画类型: 原生的 Maya 的 .mb or .ma 文件, 3ds Max 的 .max 文件, Cinema 4D 的 .c4d 文件

如何导入动画资源: 只需要将模型直接拖入 Project 视窗中的 Assetes 目录即可。选中动画资源文件，可在 Inspector 视图的 Import Setting 中编辑导入设置。

## 13.3.3 动画分解

为什么要进行动画分解: 根据不同的需求，可以将不同动作分别导入为若干个独立的动画片段, 也可以被导入为按固定顺序播放各个基本动作的单一动画片段。对于后者，必须Unity内部将其分解为1若干个子片段。

如何进行动画分解:
1. 使用预分解的动画模型

   特点: 含有预分解动画片段的模型，是 最容易使用 的

   使用方式: 导入含有预分解动画片段的模型时，动画导入面板会有所不同(⻅ P224 图 13-23)。面板中含有一个可动的动画片段列表，可单击底部 Play 按钮 预览，可根据需要，对每个片段的帧数范围进行编辑调整。

2. 使用未分解的动画模型

   如何使用：导入仅提供单一连续动画片段的模型时，导入面板与预分解动画不同(⻅ P224 图 13-24), 此种情况下，可以自行设定每个动画序列的帧数范围, 通过单击动画导入面板 Animation标签⻚中下部的 + 按钮，选中新增的动画，进而指定包含的帧数范围，设置完毕后点击 Apply 应用即可添加一个新的动画片。

3. 为模型添加动画

   为模型添加动画有几种情况: 两种，即非 Mecanim 和 Mecanim模型

   非 Mecanim模型 如何添加动画:
   - 用户可以为任意模型的动画组件添加动画片段，该模型甚至可以没有肌肉定义(非 Mecanim 模型)，进而在 Animations 属性中指定一个缺省动画片段，和所有可用的动画片段
   - 在 非 Mecanim 模型 上加入动画片段，就必须采用非 Mecanim 的方式即，将 Muscle Defination 属性设置为 None

   有肌肉定义的 Mecanim 模型 如何添加动画?
   1. 选中具有肌肉定义的 Mecanim 模型
   2. 创建一个新的 Animator Controller
   3. 打开 Animator Controller 窗口
   4. 将特定的动画片段拖入 Animator Controller 窗口
   5. 将模型资源拖入 Hierarchy 视图

---

### 13.3.4 循环播放动画片段

为什么要循环播放动画：确保动画可以很好的循环播放，是动画制作中最基本的操作之一

如何实现:  Mecanim 系统为循环播放动画片段提供了一套方便的工具，动画片段可以基于姿态，旋转，位置进行循环

使用技巧: 在动画片段的 Inspector 视图中，可以拖动动画片段的 Start 和 End 点, 拖动时可以看到一系列的循环适配曲线, 如果曲线右侧的原点显示为绿色，则可以很好的循环播放，否则为红色。

## 13.4 人形⻆色动画

---

### 13.4.1 创建 Avatar

模型的⻣骼类型：Humanoid，Generic，Legacy

指定模型的骨骼种类: 将模型导入 Assets 后，在 Project   Assets 视图中选择模型，在右侧的Inspector 面板的 Rig 选项卡中的Animation Type属性中，通过下拉菜单选择并指定它的⻣骼类型，选择后点击 Apply 即 可将其作用到模型上

1. 人形动画 Humanoid

   Humanoid 添加过程: 根据上述方法指定模型的⻣骼类型为 Humaniod 后，Mecanim 系统就会尝试将用户所提供的 ⻣骼结构与 Mecanim 系统内嵌的⻣架结构进行匹配。匹配过程通常 Mecanim系统分析⻣架的关联性并 自动完成 ，若匹配成功，在 Configure 按钮 左侧会出现一个对勾。匹配成功时 ，Project 视图中的 Assets 资源文件夹中，一个 Avatar 子资源文件将被添加到模型资源中，选择这个 Avatar 以配置子资源。此处的成功匹配， 仅指代成功匹配了所有必要的关键⻣骼 ，要达到更好的效果，需要使一些非关键⻣骼也匹配成功，并使模型处于正确的姿态 (T-pose) 还需要 对 Avatar 进行手动调整。匹配失败时，Configure 左侧的对勾会变为叉号，并在 Inspecter   Rig 选项卡中提示 Error; 此时需要对 Avatar 进行手动设置。

2. 非人形动画
   非人形动画都有哪些：一般动画类型 (Generic) 和 旧版传统动画类型 (Legacy)

---

### 13.4.2 配置 Avatar

为模型资源正确设置 Avatar 极为重要，Avatar 也是 Mecanim System 中极为重要的模块

无论 Avatar 自动创建是否成功，都需要进入 Configure Avatar 界面确认其有效性

确定有效性:  确认⻣骼结构与 Mecanim 与定义的⻣骼结构是否正确匹配，确认模型是否已经处于 T-pose

在单击 Configure 按钮时，编辑器会要求保存当前场景。因为在 Configure 模式下，Scene 视图会被占用，即用来显示当前模型的 ⻣骼，肌肉，动画信息，而不是场景信息。

保存场景后，会进入 Avatar 配置面板买中包含了一个反应关键⻣骼信息的视图，如P227 13-31

Avatar 配置面板视图作用： 显示那些⻣骼是必须匹配的(在视图中以实线圆圈表示)。可选匹配⻣骼的运动会根据必须匹配⻣骼的状态来进行自动插值计算。为了方便⻣骼匹配，用户提供的⻣架中应该包含所有必须匹配的⻣骼。

⻣骼命名规范：为了提高匹配效率，应尽量通过⻣骼代表的部位为其命名

无法自动匹配时手动配置:
1. 单击面板下方的 Pose   Sample Bind-Pose 来获得模型原始姿态
2. 单击 Pose 按钮左侧的 Mapping   Automap，基于原始姿态创建⻣骼映射
3. 单击Pose   EnforceT-pose强制模型接近T姿态
- 上述过程中如果 1，2 两步中出现映射失败，用户可以通过 Scene 视图 或者 Hierarchy 视图中拖出的⻣骼来指定⻣骼
- 如果⻣骼最终指定正确，但⻆色模型没有处于正确位置，用户会看到 Character not in T-pose 提示，此时可以通过再次 Enforce T-pose 按钮或者直接旋转⻣骼的方式将其调整到 T 姿态
- 上述⻣骼信息可以保存成一个 .ht 类型的人形模板文件，方便复用

---

### 13.4.3 设置 Muscle 参数

作用是限制⻣骼运动范围

优点：可以在 Avatar 面板的 Muscle&Setting 选项卡中调节相关参数，面板中可以非常容易地调整⻆色的运动范围，确保⻣骼运动看起来真实自然。

作用范围：可以根据需求，设置变形方法对几根⻣骼同时进行调整。可以对每根⻣骼进行单独调整。

---

### 13.3.4 Avatar Body Mask 身体遮罩

作用：通过 Mask 来控制身体的某一部分是否受动画影响

开启Mask设置：在 Project 视窗中点击一个 FBX 文件，在其 Inspector 视窗中可以找到 Mask

作用范围：Mask 可以控制身体的部分包括:头部，左右臂，左右手，左右腿，根结点，根结点以脚下的 shadow 表示

Mask功能：为手和脚切换 IK 状态，从而决定在动画混合过程中是否引入 IK 曲线，单击 Avatar 一部分来开启或关闭对应部分的 IK 功能双击空白区域来 开启或关闭所有部分的 IK 功能

如何为 Animator 或资源设置 Mask： 在 Mesh Import Inspector (在 Project 视图中点击 FBX 格式文件，其 Inspector 视图即为 Mesh Import Inspector)的 Animation 选项卡, 以及 Animation Layers (Animator -> open -> Animation Layers)面板中找到 Mask 控制选项

如何分别为 Animation 中不同片段设置 Mask：在 Mesh Import Inspector -> Animation 选项卡 -> Clips 模块中，含有所有游戏对象的动画片段。

如何创建 Mask 资源：通过 导航菜单栏 Assets -> Create -> Avatar Mask 来创建 Mask 资源。该资源以 .mask 格式的文件保存。

Mask 优点:
- 当指定 Animation Layers 时，这些 Mask 资源可以在 Animator Controllers 中被复用
- 使用 Mask 可以减少内存开销(遮罩部分不需要计算动画曲线) 同时动画回放时也不需要重新计算无用的动画曲线，进而减少 CPU 开销cc

---

### 13.4.5 人形动画的重定向

为什么要进行人物动画重定向: 人形动画重定向是 Mecanim 系统中最强大的功能之一，可以通过简单的操作，将一组动画应用到多种人形⻆色模型上

只能应用于人形模型，因此必须正确配置 Avatar

推荐配置, 推荐使用如下的层次结构:
1. 导入的⻆色模型，其中含有一个Avatar
2. Animator 组件，其中引用了一个 Animator Controller 资源 3. 一组被 Animator Controller 引用的动画片段
4. 用于⻆色动画的脚本
5. ⻆色相关组件，如 Character Controller 等

---

### 13.4.6 逆向运动学功能 IK

⻆色动画实现方式:大多数⻆色动画都是通过将⻣骼的关节⻆度旋转到预定值来实现的，子关节的位置由副节点的旋转⻆度决定。这种决定⻣骼位置的方法称为前向运动学

逆向运动学: 给定末端节点位置，从而逆推出节点链上所有其他节点的合理位置

在 Mecanim 系统中， 任何正确设置了 Avatar 的人形⻆色 都支持 IK 功能

为了设置⻆色模型的 IK，需要知道可能与之进行交互的周边物体，进而编写Ik脚本，常用的 Animator 函数包括:
- SetIKPositionWeight
- SetIKRotationWeight
- SetIKPosition
- SetIKRotation
- SetLookAtPosition
- bodyPosition
- bodyRotation

P231逆向运动学

## 13.5 动画混合

---

### 13.5.1 混合树
什么是动画混合?与动画过渡有什么区别:二者都可以生成平滑的动画。动画混合是通过插值技术实现对多个动画片段通以不同的程度平滑地混合动画过渡是在一定时间内从一个动画状态向另一个动画状态的平滑过渡

动画混合特点：每个动作对于最终结果的贡献量取决于 混合参数。动画混合树可以作为状态机中的一种 特殊的动画状态存在。

有意义的动画混合的条件: 混合的动作必须具有相似的性质和时间。

如何制作混合树?：
1. 在 Animator Controller 中右键单击空白区域
2. 在弹出的菜单中一次选择 Create State   From New Blend Tree
3. 双击视窗中新建的混合树，进入混合动画编辑界面
4. 当前⻚面会显示整个混合树的图形(可通过右键单击混合树，添加子动作和子混合树，添加后单击混合树或子混合树，在对应的Inspector视窗中可以为空白动作添加Animation)，如 P234 13-48，而属性面板显示当前选定的节点及其直接子节点。

有什么不同的混合方式?：1D混合，2D混合，直接混合

---

### 13.5.2 1D混合

在混合树的 Inspector 视图中，Blend Type 属性可以选择不同的混合方式

1D混合就是通过唯一的一个参数来控制子动画的混合，即Animation Parameter。

Animation Parameter 的取值范围：[-1.0, 1.0] 向左倾斜 ~ 向右倾斜

混合树添加动画片段：在 Animator Controller 主视图中右键单击某个混合树，选择 Add Motion。点击混合树对应的 Inspector 视图的 Motion 模块下方的 + 号。

混合树的 Parameter 如何修改：单击混合树对应的 Inspector 视图中 Parameter子视图中的蓝色金字塔，将其向左或向右拖动可 以改变动作的 Threshold(阈值)。如果未启用 Inspector 视窗下方的 Automate Threshold 切换，可以通过在 Threshold 列中的数 字来编辑 Motion 列表中的 Threshold。

Parameter 视图表示什么：表示了混合参数变化时，每个子动画的影响，其中每个子动画都用一个蓝色金字塔表示，第一个和最后一个动画只显示一半的金字塔。使用鼠标左键单击某个金字塔形状并按住不放时，相应的动画片段会在Parameter子视图下方的 Motion列表中高亮显示。每个金字塔的顶端代表该动画片段的混合权重为1，而其他所有动画的混合权重都为0。视图中红色的竖线表示当前的混合参数。

预览: 在单击 Inspector 底部的 Play 按钮后，拖动红线向左或向右移动，可以观察到混合参数对于最终动画混合效果的影响。

---

### 13.5.3 2D混合

通过两个参数来控制子动画的混合

2D混合的模式:
1. 2D Simple Directional (2D简单定向模式) 该模式适用于所有动画都具有一定的运动方向，或者其中 任何两个子动画的运动方向都不相同的情况(如向前向后向左等)
2. 2D Freeform Direction (2D自由定向模式)同样适用于具有一定运动方向的情况，且 同一方向上可以存在多个 动画
3. 2D Freeform Cartesian (2D自由笛卡尔模式)适用于动画不具有确定运动方向的情况

设置 2D 混合的动画混合树: 设置混合类型为2D后，需要选择通过哪两个 Animation Parameters 来控制混合树(如 velocity X & velocity Z，即平移速度和前进速度)。可以通过拖动 混合树 Inspector视图中的 Parameter子视图中的蓝点来改变动作的位置 还可以在 Motion列表中编辑 Pos X 以及 Pos Y 来设置动画的位置。

Inspector 中 Compute Position 的作用: 根据用户从动画剪辑中的根部动作获取到的数据来设置位置，可供选择的数据是速度或⻆速度。参数列表⻅ P237 表13-7，表13-8

修改Parameter：在混合树的 Inpsector   Parameter 视窗中，选中某个蓝色菱形后，其影响范围将通过蓝色的 可视化场来表示。蓝色菱形外的蓝色圆圈越大，说明该动画当前所占的权重就越大

预览：单击混合树 Inspector面板底部的Play后，拖动红点就可以观察到两个混合参数对于混合结果的影响，拖动红点逐渐靠近某个蓝色菱形时，其外侧的圆的直径会相应变大，其他的会变小

---

### 13.5.4 直接混合

什么是直接混合：将动画参数直接映射到子混合树的权重，可以帮助用户更精确的控制混合动画，而不是间接使用一个或两个参数

特点：用户可以将动作添加到动画列表中，然后应该为每个动作分配相应的参数，以直接控制树中的混合权重。实际上直接模式只是绕过了交叉简便，或者各种2D混合算法等，允许用户实现用代码控制混合动画的混合，可以让用户直接控制每个节点的权重，适用于脸部表情的动画混合，或者可以叠加的动画混合。

# Chapter14 Timeline

作用：创建电影内容，游戏序列，音频序列以及复杂的例子效果

特点：使用Unity的Timeline创建的每个剪辑场景，电影，或者游戏播放序列都会包含Timeline资源和Timeline实例

## 14.1 Timeline概述

使用过程中Timeline编辑器窗口会保存 Timeline Asset和Timeline instance

优点：可以在场景中直观地排列连接到 GameObject 的 Track (轨道)和剪辑中

1. Timeline Assets

   储存 Track， 剪辑，以及录制的动画，而不会链接到具体游戏对象上存在的动画，Timeline Assets 保存在 Project 中

   制作方式: 如果在创建电影，剪切场景或游戏播放序列时，录制关键动画，则 Timeline 编辑器窗口会将录制的动画保存为Timeline Asset 的子项。

2. Timeline instance

   尽管 Timeline Asset 定义了剪切场景，电影或游戏播放序列的轨道和剪辑，但无法将 Timeline Assets 直接添加到场景中。要使用 Timeline Asset 为场景中的 GameObject 创建动画，必须要创建 一个 Timeline instance

   在 Timeline 编辑器窗口中，提供了在创建 Timeline Assets 时自动创建 Timeline instance 的方 法

   在场景中选择一个具有与 Timeline Assets 关联的 Playable Director 组件的游戏对象，则 Bindings 将会显示在 Timeline 编辑窗口和 Playable Director 组件中

3. 重用TimelineAssets

   由于 Timeline Assets 和Timeline实例是分开的，因此可以在多个 Timeline 实力中重复使用同一 个 Timeline Asset

   Timeline 窗口和动画窗口的区别:
   - Timeline 窗口:

     可以在同一个序列中，只做许多不同的游戏对象或动画，可以有多种类型的轨道，切每个轨道可以包含多个可移动剪切混合的剪辑，有利于创建更复杂的动画序列，需要将多个不同的游戏对象在一起进行编排功能更新，取代了依稀动画窗口的功能

   - 动画窗口:

     可以创建单个动画片段，以及查看导入的动画片段动画片段用于存储单个游戏对象，或单个游戏对象层次结构的动画。有利于制作离散的游戏动画(旋转硬币，推⻔，摆手等)，可以更简单地创建动画片段，并未单个游戏对象创建动画，可以在动画窗口中创建片段，并使用Animator控制器进行组合和混合

## 14.2 Timeline 工作流程

---

### 14.2.1 创建 Timeline Assets 和 Timeline instance

如何使用 Timeline Assets?：使用 Playable Director 组件将 Timeline 资源关联到游戏对象上。将 Timeline Assets 与 Playable Director 关联时，会创建一个 Timeline instance，并允许用户指定 Timeline Assets 为场景中的哪些对象设置动画。（**游戏对象还必须有一个 Animator 组件**）

创建新的 Timeline Assets 和 Timeline instance:
- 在场景中，选择用作电影，或其他基于游戏的序列焦点的 GameObject
- 打开 Timeline 编辑器窗口(Window -> Timeline)，如果对象还没有附加到 Timeline 资源的 Playable Director 组件上，则 Timeline 编辑器窗口中的消息会提示用户创建。
- 单击 Create 按钮创建 Timeline 资源，对话框回提示用户正在创建的 TImeline Assets 的 名称 和位置
- 单击保存

---

### 14.2.2 使用无线剪辑录制基本动画

无限剪辑:  包含在 Timeline 编辑器窗口中，记录的基本关键动画的剪辑。没有固定大小，无法定位 裁剪 拆分，时间跨越整个动画轨道

创建无限剪辑: 当直接将动画录制到空的动画轨道时，将创建一个无限剪辑。创建之前，用户必须为想要制作动画的GameObject添加一个空的动画轨道在轨道列表中，单击空白轨道的录制按钮以启用录制模式


# Chapter15 UGUI

## 15.1 概述

UGUI 是帮助用户快速直观地创建图形用户界面

## 15.2 Canvas 画布

---

### 15.2.1 Canvas

是存放所有 UI 元素的容器;所有 UI 元素都必须放在画布子节点下

通过 GameObject UI 下的子项创建 GUI 控件时，如果当前不存在画布，系统会自动创建一个画布

画布的渲染模式：
1. Screen Space-Overlay:
   使画布拉伸以适应全屏大小。使 GUI 控件在创建中渲染于其他物体的前方画布的大小会根据屏幕大小和分辨率的变化而变化
2. Screen Space-Camera
   画布 以特定的距离放置在指定的相机前。UI 元素被指定的相机渲染，其呈现会受相机设置的影响
3. World Space
   使画布渲染于世界空间该模式下，画布在场景中与其他游戏对象一样，可以手动调整Rect Transform 来改变画布大小 GUI 控件可能会渲染于其他物体的前方或后方。
4. UI Scale Mode
   UI 的缩放模式，在 Canvas Scaler 组件中有如下参数:
   - Constant Pixel Size: 固定的像素大小
   - Scale With Screen Size
   - Constant Physical Size:固定的物理大小(厘米，毫米等)

Graphic Raycaster(Script)图形检测组件作用：用于对 Canvas 进行射线检测。

Raycaster 会查看画布上的所有图形，并确定是否有图形已被击中。参数如下:
- Ignore Reversed Graphic:是否忽略背面的图形检测
- Blocking Objects:阻挡图形射线检测的对象的类型
- Blocking Mask:阻挡图形射线检测的遮罩层

---

### 15.2.2 Canvas Group

使用 Canvas Group 可以对 UI 元素进行分组，方便同一控制和管理

在 Inspector 中点击 Add Component 按钮后，搜索Canvas Group并添加

参数:
- Alpha: 可以统一调节改组所有UI元素透明度
- Interactable: 控制该组件是否受输入控制
- Block Raycasts: 控制该组件是否作为碰撞起的 RayCasts。不适用于Physics Raycast，当要处理 Canvas 上 UI 元素的 RayCast 时，应调用绑定在 Canvas 上的 Graphic Raycaster 组件的 RayCast 方法。
- Ignore Parent Group: 用于控制是否忽略父对象上的 Canvas Group设置

---

### 15.2.3 元素绘制顺序

UI 元素的绘制顺序依赖于它们在 Hierarchy 面板中的顺序

如果两个 UI 元素重叠，后添加的 UI 元素会出现在之前添加的元素的上面

调整 UI 绘制顺序:
- 通过在 Hierarchy 中拖动元素进行排序
- 通过 在脚本中控制 Transform 组件上的: SetAsFirstSibling，SetAsLastSibling，和 SetSiblingIndex 等方法实现

## 15.3 EventSystem 对象

当UGUI的第一个 Canvas 被创建时，Hierarchy 视图中会自动创建一个 Event -System 对象

包含:
- Event System:用来管理 UI 的事件系统
- Standalone Input Module:独立的输入模块

在处理 UI 的交互上，EventSystem 对象上是必不可少的。如果没有 EventSystem对象，那么 UI 对象就无法处理事件和交互

创建 EventSystem 对象: 点击菜单栏中的 GameObject -> UI -> Event System

---

### 15.3.1 Event System 组件

Event System 组件的作用: 该组件负责控制所有 UI 元素的事件，它的当前坐标在输入模块上，每次 Update 时，都会调用 Event System。调用时，通过输入模块和在输入模块里的计算输出标记，将处理的委托返回给本模块

---

### 15.3.2 Standalone Input Module 组件

用于设计控制器鼠标输入的工作。按键按下拖动以及类似的事件会发送到响应输入中。该组件通 过输入管理器来发送移动事件，提交取消事件的响应输入。跟踪轴和键值可以通过该组件的属性进行配置。

## 15.4 基本布局

---

### 15.4.1 矩形工具

在 Scene 视图中，使用矩形工具可以平移，旋转，缩放 GUI 控件。

选择一个 UI 元素后，单击工具栏中的矩形工具按钮。可以在控件内的任意位置单击并拖动来改变它的位置，可以在控件的边⻆单击拖动改变其大小，当鼠标指针悬浮在拐⻆附近时，鼠标指针右下方变成一个旋转符号时，可以按住后朝任意方向拖动，以旋转控件。

---

### 15.4.2 矩形变换 Rect Transform

一种新的变换组件，适用于在所有的 GUI 控件上来替代原有的 Transform 组件

为了调整布局，一般建议调整 UI 元素的大小，而不是对其进行缩放。因为这样不会影响字体大小，切片图像的边界大小等。

Rect Transform 与 Transfrom 的区别:  在 Scene 中， Transform 组件表示一个点，Rect Transform 表示一个可容纳 UI 元素的矩形，且矩形变换还有锚点，轴心点的功能。

---

### 15.4.3 Anchors 锚点

如果一个 Rect Transform 的父对象也是一个 Rect Transform，那么作为子物体的矩形变换可以 通过多种方式固定在父物体的矩形变换上。

子物体可以固定在父物体的中心点或者某一个拐⻆处；在固定锚点时，也允许给予父对象的高或宽按指定的百分比进行拉伸。

Scene 中锚点形状: 四个三⻆形手柄的样式(⻓等腰三⻆形)

锚点的意义: 每个锚点都对应固定于相应父物体的矩形的⻆。

如何使用: 可以单独拖动每一个锚点，当它们在一起的时候，也可以单击它们的中心一起拖动。当按下 Shift 键 拖动锚点时，矩形相应的⻆会跟随锚点一起移动。

如何设置：在 Inspector 视图中，锚点预置按钮在矩形变换组件的左上⻆，单击该按钮可以打开预置锚点的下拉列表，便捷的选择常用锚点选项，可将 GUI 控件固定在父物体的某一边或中心，或拉伸到与父对象相同的大小水平方向和竖直方向的锚点时相互独立的。

在锚点预置列表里，”Shift + 预置“ 可以设置 UI 轴心点。“Alt + 预置” 可以设置 UI 的位置

---

### 15.4.4 Pivot 轴心点

旋转和缩放都围绕轴心点发生变化，所以轴心点的位置影响旋转和缩放的结果

---

### 15.4.5 补充

蓝图模式：表示是否忽略掉物体的旋转。启用时不能对物体进行旋转

原始的编辑模式：表示当修改 Anchors 时，UI 的位置及尺寸是否会根据Anchors进行匹配


## 15.5 Text 文本

---

### 15.5.1 Text 介绍

显示非交互文本，也可以作为其他 GUI 控件的标题或者标签，也可用于显示指令或其他文本

参数：⻅ P286 表15-4

---

### 15.5.2 Rich Text

当该选项启用时，标记元素中的文本将被视为样式信息，所以可以有一个单词或短语采用黑体或 不同的颜色

## 15.6 Image 图像

用于显示非交互式图像，在其他空间中也可以通过控制脚本来改变 Image控件图像

与Raw Image 区别：控件类似于 Raw Image，Image 提供了更多选项的动画控制和准确的填充控件的功能 Image 需要 Sprite 类型的纹理，Raw Image 可以接受任何类型的纹理。

参数: P287表15-6

Image Type包含的设置项:
- Simple:默认情况下适应控件的矩形大小。如果启用 Preserve Aspect，图像的原始比例将会被保存 剩余的未填充的矩形将会被空白填充
- Sliced: 图片会被切成九宫格模式。图片的中心会被缩放以适应矩形控件，边界仍会保持原有尺寸，禁用 Fill Center 后图像的中心会被挖空。
- Tiled: 图像会保持原始大小。如果控件大小大于原始图像，图像会被会重复填充，控件大小大于原始图像，图像会在边缘处截断。
- Filled: 图像显示为Simple类型。可以通过调节填充模式和参数使图像呈现出 从空白到完整填充的过程。

## 15.7 Raw Image 原始图像

用来显示非交互图像，可以用于装饰或图标等。可在其他控件中通过脚本来改变原始图像

参数中的 UV 属性作用：UV 属性允许显示一个较大图像的一小部分

## 15.8 Mask 遮罩

是一种不可⻅的 UI 控件，可以用来修饰控件子元素的外观。遮罩将子元素限制为父物体的形状，超出部分将不显示。

在 Inspector 视图中单机 Add Component 按钮后搜索 Mask 即可添加。Mask(Script) 常与 Image (Script) 控件组合使用

Show Mask Graphic:表示是否绘制该组件上的图形

## 15.9 过度选项和导航选项

---

### 15.9.1 Transition 过渡选项

在 Inspector 视图中单击 Add Component，搜索 Selectable 并添加

参数：⻅ P289 表 15-8， 15-9

---

### 15.9.2 Navagation 导航选项

控制 UI 控件的键盘导航如何实现

在 Inspector -> Selectable 组件中，单击 Navigation选项下的 Visualize 按钮，可以在Scene视 图中可视化导航选项。

Button 或 Selectable 的导航可以按键盘 方向键 进行切换

Input Field 之间的导航按 方向键 + Enter 键 组合进行切换

## 15.10 Button 按钮

响应事件:
- 在 Button 的 Inspector 中单击 OnClick 下的 + 按钮(可视化创建)
- 通过脚本监听事件绑定
- 通过 Event Trigger 实现
P290 - 293

## 15.11 Togggle 开关

允许用户选中或取消某个选项的复选框。绑定响应事件参照Button

## 15.12 Slider 滑动条

允许用户通过鼠标从一个预先确定的范围选一个数值。绑定响应事件参照Button

## 15.13 Scrollbar 滚动条

允许用户滚动因图像或其他可视物体太大而不能完全看到的视图。 Slider 用于选择数值，Scrollbar 用于滚动视图

## 15.14 Dropdown 下拉列表

P298

## 15.15 Input Field

可以使输入内容不可⻅的 UI 控件

P301

## 15.16 Scroll View 滚动视图

当内容空间大于显示区域时，利用滚动来显示其他位置里的内容

## 15.17 自动布局组件

布局元素可以灵活地控制元素尺寸

- Layout Element
- Content Size Filter
- Aspect Ratio Fitter
- Horizontal Layout Group
- Vertical Layout Group
- Grid Layout Group


# Chapter16 音效和视频

## 16.1 音效系统

---

### 16.1.1 概述

音效系统基本理论：由多普勒效应可知，对于观测者来说快速移动的声源发出的频率，会随着声源与观测者间距离的变化而变化。

如何实现模拟声音效果：Unity 要求声源是附加在物体上的音频源(Audio Source)，且发出的声音被附在另一个物体上的音频监听器接收，音频监听器通常附加在主相机上。

Unity音效系统如何实现回声：不能纯粹从场景中计算回声，但用户可以通过向对象添加音频过滤器来模拟它们。例如，通过将 Echo 过滤器应用于洞穴内播放的声音在物体可以移入和移出，且具有强回声的地方，可以向场景添加混响区域。

**Unity 支持的音频格式**：
- AIFF
- WAV
- MP3
- Ogg
- MOD
- IT
- S3M
- XM

其中AIFF，WAV 格式的短音频的声效适合本地加载使用(音频大但无需解码)。Windows 和 macOS 适合用OggVorbis格式的音频，其音质不会降低。移动平台适合用 MP3格式，非MP3格式会被压缩成MP3，该格式音质较低。

---

### 16.1.2 常用组件

----

#### 16.1.2.1 Audio Clip 音频剪辑

音频剪辑包含音频源使用的音频数据

Unity支持什么种类的音频资源：单声道，立体声，多声道。可以以 .xm, .mod, .it 和 .s3m 格式导入跟踪器模块

跟踪器模块：尽管资源导入属性中没有可用的波形预览，但 TrackModule 跟踪器模块资源的行为方式与 Unity 中的其他音频资源相同

----

#### 16.1.2.2 Audio Listener 音频监听器

充当类似⻨克⻛的设备，接收来自场景中任何给定音频源的输入，并通过计算机的扬声器播放声 音

适用情况：对于大多数程序，都可以讲音频监听器附加到主相机上。可以位于混响区域的作用范围内(混响适用于场景中所有可听到的声音)，音频效果可以应用于 Audio Listener，也可以应用于场景中的所有可听⻅的声源。

**在一个场景中，同一时刻只能有一个 Audio Listener**

----

#### 16.1.2.3 Audio Source 音频源

用来播放场景中的音频剪辑，音频剪辑可以通过音频监听器播放，也可以通过音频混音器播放。

可以播放什么类型的音频剪辑：任何类型，并且可以配置为播放 2D，3D或混合(Spatial Blend)，音频可在扬声器之间展开，并在 2D和3D之间混合(通过衰减曲线控制距离)。

---

### 16.1.3 Audio Mixer 音频混合

----

#### 16.1.3.1 概述

什么是音频混合： Audio Mixer 是 Audio Sources 可以引用的资源。Audio Mixer 允许混合各种音频源，对它们应用效果以及执行控制

1. 音频混合视图

   打开音频混合: Window -> Audio Mixer

   视图显示: Audio Mixer 窗口显示音频混合器(树状音频混合器组)

   音频混合器: 本质上是音频混合。是一个信号链，允许用户在处理音频信号和更改效果参数时插入效果 具有发送和返回机制，可将结果在总线之间传递(1对1)

   视图功能: ⻅ P311 图16-6

2. 音频混合属性

   ⻅ P311 图 16-7

3. 概念

   - 路由和混合:

     音频路由: 接收多个输入音频信号，并输出一个或多个输出信号的过程。这里的术语信号，是指数字音频数据的连续流，其可以分解成数字音频通道

     功能: 内部通常有一些与信号相关的工作，如混合，应用效果，衰减等

     特点: 除了发送和返回外，Audio Mixer 还包含允许任意数量的输入信号，混合这些信号并组成具有1 个输出的音频组

4. 声音类别

   **P312**

5. Snapshots 快照

   允许用户捕获 Audio Mixer 的状态，并在游戏进行时，在这些不同状态之间进行切换，有助于 定义情绪或主题，影响玩家情绪

----

#### 16.1.3.2 Audio Mixer 窗口详解

Window -> Audio Mixer

1. Mixers 混合面板

   显示：所有 Audio Mixer 的完整列表

   如何将Audio Mixer路由到另一个Audio Mixer 的 Audio Group:

   - 在混合面板中操作，在编辑器中更改 Audio Mixer 的输出，单击 Audio Mixer，拖动到另一个 Audio Mixer 的顶部。
   - 弹出对话框，选择要路由的目标 Audio Mixer 的 Audio Group
   - 选择后，面板将显示 Audio Mixer 的父子关系。并在 Audio Mixer 名称旁边显示其目标 Audio Group

   如何创建新的 Audio Mixe：单击 Mixer 面板右上方的 + 号

2. 将 Audio Mixers 路由到其它的 Audio Mixers

   默认情况下，每个 Audio Mixer 将音频信号直接输出到 AudioListener

   路由方式:
   - 在混音器面板的编辑器中实现
   - 在运行时使用 Audio Mixer API 动态实现

3. 层次面板(Groups)

   显示用户自定义 Audio Mixer 的声音类别和混合结构的位置。允许用户定义自己的 Audio Sources，可以连接和播放的自定义类别

4. 在层次结构中添加和配置音频组

   在何处添加和修改 Audio Mixer 的拓扑结构：在 Audio Group 层次结构面板中完成如下步骤

   添加方式有两种:
   - 右键单击现有的 Audio Group(已有至少一个Audio Group的情况下)，选择 Add child group 或 Add sibling group。
   - 单击 Groups 面板右上⻆的 + 按钮

   更改方式: 将一个Audio Group 拖动到另一个 Audio Group 的顶部，可以修改 Audio Mixer 的拓扑结构，这将使目标 Audio Group 在所选择的一个以上

   删除方式: 选中一个 Audio Group 后，单击键盘 Delete 键。或者右键要删除的组，选择 Remove group

   复制方式: 右键单击某个 Audio Group，选择 Duplicate group。该操作将完全复制该 Audio Group，包括其中的效果

   重命名方式: 右键单击，选择 Rename。或者选中后单击 F2 键

5. 音频组视图

   位置: Audio Mixer 视窗的右半部分

   结构: 竖条 Slider 调节每个 Group 的音量(垂直VU表)，VU表下方为三个按钮，SMB，按钮下方为 DSP 效果单元。

   SMB作用: S: Solo, M: Mute, B: Bypass(允许用户绕过或启用 Aduio Group中的全部效果)

   DSP 效果⻅ P315 图 16-14

6. 快照面板 Snapshot

   允许用户在 Audio Mixer 内创建，切换，调整不同的快照。始终至少有一个快照处于活动状态，在面板中的快照选择表示 Audio Mixer 的进一步编辑将对该快照进行编辑。面板中定义的快照，也显示为 Audio Mixer 的子资源，允许用户访问编辑器和脚本中的其他位置的快照。

   星号意义：代表用户自定义的开始快照 Start snapshots，在Audio Mixer加载时初始化

   创建快照：单击快照面板右上⻆ + 号，输入新快照的名称，要定义不同的开始快照: 右键单击所需的快照，选择Set as start Snapshot

7. 视图面板Views

   作用：
   - 允许用户在 Audio Mixer 中创建可⻅的 Audio Group
   - 有了视图，用户可以创建对 Audio Mixer 感兴趣的视⻆，而非始终显示完整的层次结构
   - 仅用于优化工作流，并不影响运行时的设置或性能

   操作：
   - 添加新视图:Views面板右上⻆ + 按钮
   - 更改显示:选择不同的视图，更改当前显示视图
   - 删除视图:右键单击，选择 Delete
   - 复制视图:使用所有当前视图设置，右击选择Duplicate

   Audio Group 的 Eye 图标作用：显示 or 隐藏

----

#### 16.1.3.3 音频组属性

1. Inspector Header
2. Edit in Playmode
3. Pitch Slider
4. Attenuation Unit
5. Effect Units
6. Send Units
7. Receive Units
8. Duck Volume Unit
9. 常用选项
10. Exposed Parameters
11. Transition Overrides
12. Audio Mixer

P317 - P321

---

### 16.1.4 Audio Filters 音频过滤

1. Audio Low Pass Filter
   音频低通滤波器，传低频去高频
2. Audio High Pass Filter
   音频高通滤波器，传高频去低频
3. Audio Echo Filter
   音频回声滤波器，在给定的延迟时间后重复声音(衰减比)
4. Audio Distortion Filter
   音频失真滤波器，使 Audio Source 的声音失真或声音到达 AudioListener
5. Audio Reverb Filter
   音频混响滤波器，采用音频剪辑使其变形以创建自定义混响效果
6. Audio Chorus Filter
   音频合唱滤波器，创建合唱效果

---

### 16.1.5 Audio Effects 音频效果

通过音频效果修改音频混合器组件的输出，改变声音的频率范围或应用混响

---

### 16.1.6 Microphone ⻨克⻛

从计算机或移动设备的⻨克⻛中捕获语音输入

## 16.2 音频播放器


# Chapter17 全局光照

## 17.1 概述

全局光照，简称 GI

作用：用来模拟光的互动和反弹等复杂行为的算法

两个系统：Enlighten & Progressive Lightmapper。通过 Lighting 窗口的 Lightmapper 进行切换

设置全局光照: Window -> Lighting -> Setting

---

### 17.1.1 Enlighten

通过GI算法实现实时全局光照，消耗较少性能提供更真实丰富的光照效果，提供全系的光照流程，提供了 更快的迭代模式，需要更高品质和细节时，场景会被预计算与烘焙效果替换。

优点：让用户实时看到光照结果，但任何图形的变动都要对场景重新烘焙

---

### 17.1.2 Progressive Lightmapper

渐进光照贴图，一种无偏移的蒙特卡洛方法路径追踪器，可以配合全局光照使用烘焙光照贴图，改善场景光照烘培工作流程。

优点：健壮性更高，间接以光照贴图的全分辨率进行烘焙，下次更少，可以轻松预测渲染所需的时间，进度条上的倒计时可以呈现给用户。可以随时停止烘焙，并在添加或增设内容及样本后继续烘焙。渲染速度不一定比 Enlighten 快，但从烘焙到得到视觉反馈的时间显著缩短。

---

### 17.1.3 Lightmap seam stitching

光照贴图缝合技术，可以平滑烘焙光照贴图渲染的 GameObject 中不需要的硬边缘

作用: 与 Progressive Lightmapper 一起用于光照贴图烘焙，仅适用于单个 GameObject。

在GameObject启用缝合：在 GameObject 的 Mesh Render 组件中，打开 Lightmao Settings 部分(仅当用户使用渐进式光照贴图 Progressive Lightmapper 时才可以访问) 然后勾选 Stitch Seams。

## 17.2 实践

烘焙光照的方式：Mixed 混合 & Baked 烘焙

Mixed 和 Baked 区别?
- Mixed:
  提供介于实时和 Baked 之间的光照方式，将间接光照烘焙到贴图，并始终提供直接光照动态物体阴影是实时的
- Baked:
  将光源的直接光照和间接光照都烘焙到光照贴图中，动态物体无法产生阴影

什么光照系统可以使用烘焙：Lightmapper 设置为 Progressive 或 Enlighten 时都可以进行烘焙流程

Auto Generate 作用：默认勾选，如果场景中参数变化，会自动重新生成光照贴图。取消勾选时，在用户需要重新烘焙时，手动生成光照贴图。

光源类型设置为 Baked 后，在此烘焙光照贴图，然后关闭光源，此时动态游戏对象无阴影

## 17.3 系统参数详解

---

### 17.3.1 FBX模型导入设置

导入时注意事项：确保模型的 UV 值在 0.0 到 1.0 之间，否则无法对该模型进行烘焙，烘焙时提示警告。

如何解决：在 Project 视图下 Assets 文件夹中选择模型实例对应的 FBX 文件，在 Inspector 视图中 Import Settings 面板下勾选 Generate Lightmap UVs，单击 Apply 按钮应用设置。

---

### 17.3.2 Reflection Probe 反射探针

像一个捕获其周围各个方向的球形摄像机，从四面八方捕捉周围环境的球状影像将捕获的图像存储为一个立方体贴图，可供具有反射材质的物体使用。

特点：同一个给定的场景或对象，可以添加几个反射探针。可以设置为使用 距离最近的反射探针生成的立方体贴图，物体上的反射可以根据环境变化。

添加反射探针: GameObject -> Light 中，选择 Reflection Probe。

面板作用: 在 Inspector 的 Reflection Probe 面板上部有两个按钮，分别由编辑探针大小，和修改探针在场景中位置属性的功能。

---

### 17.3.3 Light Probe Group 光照探针组件

一种快速计算实时渲染应用中的光照技术，常用于处理游戏世界的人物⻆色或是动态物体的光照，允许移动对象接受由全局光照所计算出来的复杂反射光源。

优点：在运行时有不错的处理性能 (消耗低)，而且预计算也相当快速。

特点：如果没有添加光照探针，动态对象就无法接受全局光照

注意事项：
- 密度不应太高
- 距离太近的光照探针在特定光照条件下的采样结果几乎一致
- 推荐在光照变化明显的区域设置密度较高的探针

---

### 17.3.4 Lighting 窗口

如何打开 Lighting 窗口：Window -> Lighting -> Settings

作用：实时 GI 开销较大，Lighting窗口允许用户根据需要调整光照过程，如定制用户的场景或优化质量，提升质量和分配储存空间，同时包含照明相关的设置，包括环境光，天空盒，雾效等。

Auto Generate：不论切换 Scene， Global maps 还是 Object maps，它始终在底部启用时，光照贴图随着用户编辑的场景更新。关闭时，Generate Light 复选框激活，需要使用按钮手动触发更新，Generate Light 按钮下拉菜单中有一个选项可以清楚场景烘焙的数据 (不清除 GI 缓存)。

**环境参数**：重点，⻅ P342 表 17-3 (实时光照，混合光照，光照贴图参数*)

---

### 17.3.5 Light Explorer 光探测器

允许用户选择和编辑光源

Window -> Lighting -> Light Explorer


# Chapter18 导航网格寻路 Nav Mesh

## 18.1 Unity的导航寻路系统

导航网格： Nav Mesh 是 3D游戏世界中用于实现动态物体自动寻路的一种技术，它将游戏场景中复杂的结构组织关系简化为带有一定信息的网格，在这些网格的基础上通过一系列的计算来实现自动寻路。

如何使用导航网格：系统可以根据用户所编辑的场景内容，自动的生成导航网格。实际导航时，只需要给导航物体挂载导航组件，导航物体变便会形根据目标点来寻找符合条件的路线，并沿着该路线行进到目的地。

Unity Nav Mesh组成：

1. Nav Mesh：
   - 导航网格
   - 描述游戏世界的步行表面的数据结构
   - 允许从游戏世界两点间，生成一个可以行走的路径
   - 数据结构是根据关卡自动生成或烘焙的

2. Nav Mesh Agent：
   - 导航网格代理
   - 代理组件可以帮助用户创建⻆色
   - 代理使用 Nav Mesh 对游戏世界进行推理
   - 知道如何避开彼此和移动的障碍物

3. Off-Mesh Link：
   - 非网格连接组件
   - 允许 Agent 不按照 Nav Mesh 进行移动

4. Nav Mesh Obstacle：
   - 导航网格障碍组件
   - 用于描述运动的物体
   - Agent 会有选择地绕过它，从而避免与之碰撞或穿透

## 18.2 实践操作

P347

- 添加导航网格

  选中对象，在 Inspector视图右上⻆static下拉列表中选择 Navigation Static。此时，对象标记为 Navagation Static

  Window -> Navigation

  在 Navigation 窗口中单击 Bake选项卡 右下⻆的 Bake按钮生成 Nav Mesh

  烘焙完成后会在 Assets 中自动创建一个 NavMesh 目录

- 添加 Agent

  选择游戏对象，Inspector -> Add Component -> NavMesh Agent

  或者

  Component -> Navigation -> NavMesh Agent

  添加完成后，对象上会出现绿色的圆柱框，绿色圆柱框即为 Navigation 视窗中的 Baked Agent Size

- 为游戏对象添加材质

  Assets -> Create -> Material

- 实现跳跃

  在 Navigation 视窗中，编辑 Generated Off Mesh Links 的两个参数，Drop Height 和 Jump Distance，之后重新Bake即可。**注意，设置的 Drop Height 应比场景中测量的高度值大一些，以便非网格连接正确**

## 18.3 系统参数详解

---

### 18.3.1 Navigation 窗口

Window -> Navigation

面板属性：

1. Object 物体参数面板

   - Navigation Static: 勾选后，该游戏对象将参与导航网格的烘焙
   - Generate Off MeshLinks: 勾选后，自动根据 Drop Height 和 Jump Distance 的参数设置，用关系线来连接分离的网格
   - Navigation Area: 导航区域设置。在默认情况下分为 Walkable，Not Walkable，Jump

2. Bake 烘焙参数面板

3. Areas 导航区域设置，用于对导航网格分层

4. Agents 代理设置

   - 默认只能由 Humanoid 代理烘焙出 Nav Mesh
   - 为了将导航网格烘焙成其他代理类型，需要使用 NavMesh Sur法测组件

---

### 18.3.2 Nav Mesh Agent

---

### 18.3.3 Off Mesh Link

---

### 18.3.4 Nav Mesh Obstacle

注意:如果 Nav Mesh Obstacle 未勾选 Carve 复选框，当⻆色寻路有障碍物阻挡时，将不会自动绕开，而是处于被阻挡状态

## 18.4 导航网格寻路的高级技巧

---

### 18.4.1 使用 Off Mesh Link

作用: 当用户不需要在 Navigation 窗口中生成的多条非网格连接时，可以使用 Off Mesh Link 组件实 现

使用方式:
- 在 Navigation 视窗 Bake 选项卡中，将 Drop Height 和 Jump Distance 设置为 0;
- 创建一个空对象，命名为 Link，给它添加一个 Off Mesh Link 组件(Component   Navigation);
- 创建一个空对象，命名为 end，将 end 设置为 Link 的子物体，将 Link 上的 Off Mesh Link 组件的 Start 设置为 Link，End 设置为 end
- 同理，其他地方也可以添加非网格连接
- 运行游戏，即可通过非网格连接寻路

---

### 18.4.2 为网格分层

Navigation -> Area -> Add Area “Bridge”

Hierarchy -> Bridge(1) -> Navigation -> Object -> Navigation Area 设为 Bridge

---

### 18.4.3 动态更改可行进层

---

### 18.4.4 使用 Nav Mesh Obstacle


# Chapter19 遮挡剔除

## 19.1 概述

遮挡剔除技术: 当一个物体被其他物体遮挡住，而相对于摄像机不可⻅时，可以不对其渲染

重复渲染 overdraw: Unity 引擎不会自动进行遮挡剔除，因多数情况下离相机远的物体先渲染，近的物体后渲染，从而覆盖先渲染的

与视锥体剔除(Frustum Culling)的区别: 视锥体剔除只是不渲染摄像机视锥之外的物体，被遮挡的物体依然会被渲染，使用遮挡剔除功能时，视锥体剔除功能依然有效

## 19.2 参数详解

---

### 19.2.1 Occlusion 窗口

Window -> Occlusion Culling

遮挡剔除窗口功能: 窗口的 Object 选项卡中，选中场景中的网格渲染器，可修改静态标志
- Occluder Static:开启该标记的物体，既能遮挡，也能被遮挡
- Occludee Static:开启该标记的物体，只能被遮挡

选择 Occluder or Occludee:
1. 选中对象，Inspector -> Static 下拉列表 -> 设置 Occluder， Occludee
2. 选中对象，Occlusion -> Object 勾选

Occlusion Area: 在 Occlusion 视窗中可以选择遮挡区域，默认遮挡剔除应用于整个Scene。⻅ P362

Occlusion Bake 选项卡： P361


# Chapter20 后期屏幕渲染特效

## 20.1 概述

后期处理：将全屏过滤器和效果应用于相机的图像缓冲区，并将其显示到屏幕上，可以在短时间内大幅提升产品的视觉效果

效果：
- Bloom 泛光
- Depth of Field 景深
- Chromatic Aberration 色差
- Color Grading 颜色分级

后期处理栈及其优点:

可以将一组完整的效果合并到一个后期处理管道中

- 效果总是按正确顺序配置
- 允许将多种效果组合成单通道
- 所有效果都组合在用户界面中

包含一组监视器(Monitors)和调试视图(Debug Views)

使用后期处理: 从Asset Store 中下载 Post Processing Stack 并导入

注意事项: 为获得最佳的后期处理效果，建议在启用 Allow HDR 的线性色彩空间中工作, 也建议使用延迟渲染路径。

设置 Post Processing Stack：

1. 将PostProcessingBehaviour.cs脚本添加到相机上

   - 将脚本从 Project 视图拖动到相机上
   - 依次点击 Component   Effects   Post-ProcessingBehaviour
   - 或使用 Inspector 视图中的 AddComponent按钮

2. 使用以下方法之一创建自定义配置文件

   - 右键单击 Project -> Create -> Post-Processing Profile
   - Assets -> Create -> Post-Processing Profile

   Tip:后期处理配置文件是项目资源，可以在场景相机项目/商店之间轻松共享

## 20.2 参数详解

---

### 20.2.1 Fog 雾效

雾效：是根据与相机之间距离，将颜色叠加到物体上的效果,用于模拟室外环境中的雾效, 根据相机的深度纹理创建屏幕空间雾效,支持线性，指数，指数平方雾类型

设置：在 Lighting 窗口的 Scene 选项卡中设置

注意事项：此效果仅适用于延迟渲染路径(Deferred)，雾效应用在向前渲染 (forward rendered) 物体上，并使用场景设置中的雾效

---

### 20.2.2 Anti-aliasing 抗锯⻮

抗锯⻮：Anti-aliasing 提供了一组算法，可以防止锯⻮以提供更平滑的外观，VR 中不支持抗锯⻮

VR 中不支持抗锯⻮：

- Fast Approximate Anti-aliasing(FXAA)：
  快速近似抗锯⻮，最经济的技术，推荐用于不支持运动矢量的移动平台等，也适合作为较慢桌面系统和控制台硬件的备选方案。
- Temporal Anti-aliasing (TAA)：
  时间消除锯⻮，一种更高级的锯⻮消除技术，将帧累计在历史缓冲区，以便更有效地平滑物体边缘，在平滑运动边缘方面效果更好，但需要运动矢量，计算开销更大。

---

### 20.2.3 Ambient Occlusion 环境光遮罩

作用：可实时逼近全屏后期处理效果，使得互相靠近的折痕，孔，交叉点变暗，现实生活中这些区域往往有遮挡或遮挡环境光线，因此看起来较暗

特点：环境光遮罩计算开销很大，通常只能在桌面或控制台硬件上使用

---

### 20.2.4 Screen Space Reflection 屏幕空间反射

作用：是一种重新使用屏幕空间数据来计算反射的技术，通常用于创建更加微妙的反射(潮湿的地板或水坑)

特点：计算开销大，但效果很好，不建议在移动设备上使用，仅在于延迟渲染路径中可用

---

### 20.2.5 Depth of Field 景深

作用：可模拟相机镜头的对焦属性，焦点远处的物体会失焦

---

### 20.2.6 Motion Blur 运动模糊

作用：模拟相机在拍摄的物体移动速度快过相机曝光速度造成的模糊

---

### 20.2.7 Eye Adaption 眼部适应

作用：模拟眼睛适应不同程度黑暗和光线的能力，此效果会根据其包含的亮度级别范围，动态调整图像的曝光，调整是在一段时间内逐渐进行的。

---

### 20.2.8 Bloom 泛光

作用：用于再现真实世界相机的成像伪影的效果(光晕)

---

### 20.2.9 Color Grading 颜色分级

作用：改变或校正最终图像的颜色和亮度的过程，可看作成像在照片处理软件中使用过滤器

---

### 20.2.10 User Lut

作用：一种更简单的颜色分级方法，比颜色分级更先进，此方法不需要 在Color Grading 中使用的 高级的纹理格式

---

### 20.2.11 Chromatic Aberration 色差

作用：用于复制相机的缺陷，如无法将所有颜色聚焦到同一点

---

### 20.2.12 Grain 颗粒

作用：胶片颗粒是照相胶片中的金属银颗粒产生的随机光学纹理，模拟电影的某些效果

---

### 20.2.13 Vignette 渐晕

作用：模拟与中心相比，图像边缘变暗/去饱和的效果，常用语产生艺术效果，如将焦点集中到图像中心

---

### 20.2.14 Dithering 抖动

作用：模拟与中心相比，图像边缘变暗/去饱和的效果，常用于产生艺术效果，如将焦点集中到图像中心

---

### 20.2.14 Dithering 抖动

作用：有意施加噪声，以随机量化误差，防止图像中出现大规模的颜色条纹

---

### 20.2.15 Debug Views 调试视图

作用：可以查看特定的效果或路径

---

### 20.2.16 Monitors 监视器


# Chapter21 Shader 开发

## 21.1 Shader 概述

什么是 Shader： 着色器，用来控制可编程图形渲染管线的程序

作用：替代了传统的固定渲染管线，可以在渲染管线中应用3D图形学的相关计算，极大地拓展创作者的开发空间

Unity Shader 特点：基于物理的 Standard Shader，可以创建出非常多的不同材质，不需要身后的 3D 图形学知识，也可以做出基于物理渲染的真实效果。

PBS：基于物理的着色，Physically Based Shading 简称PBS，遵从了 conservation of energy 能量守恒定律的理论。可产生自然和谐的光照效果。

## 21.2 内建 Shader 介绍

P387 - 389

---

### 21.2.1 内建着色器

---

### 21.2.2 内建标准着色器

## 21.3 Shader 的创建

Shader种类：

- Surface Shader:

  表面着色器，通常使用这种 Shader，可以与灯光，阴影，投影器进行交互，使用 Cg/HLSL 编写。

- Vertex and Fragment Shaders:

  顶点和片段着色器，不需要与灯光进行交互，更灵活，代码量更大，很难与渲染管线完美集成，使用 Cg/HLSL 编写。

- Fixed Function Shaders:

  固定功能管线着色器，可在不支持可编程管线的老旧硬件上运行，使用 ShaderLab 编写。

SubShader：子着色器，当 Unity 使用着色器渲染时，会从上到下遍历子着色器，找到第一个能被用户设备支持的着色器，并用其进行渲染。

FallBack：备选着色器，一般会指定一个对硬件要求最低的 Shader，当所有子着色器都不能运行时，Unity 会使用备选着色器进行渲染。


# Chapter22 AssetBundle 工作流程

支持在游戏运行过程中，对资源进行动态下载和加载，是 Unity 提供的一种用于存储资源的文件格式 可以表示彼此间的依赖关系，可用于下载内容(DLC)。

## 22.1 AssetBundle 的创建

通过 AssetBundle 的 UI 和简单的脚本，在 Unity 中创建 AssetBundle 文件

API:BuildPipeline.BuildAssetBundles

注意事项：AssetBundle 的标记名称要小写，可以有后缀


# Chapter23 多人游戏和联网

其中重点看 23.9 Unity 服务重点浏览