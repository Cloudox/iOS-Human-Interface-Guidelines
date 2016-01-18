# iOS-Human-Interface-Guidelines
翻译自苹果官方文档《iOS Human Interface Guidelines》

## 目录
* [UI Design Basics](#UI Design Basics)
  * [Designing for iOS](#Designing for iOS)
  * [iOS App Anatomy](#iOS App Anatomy)
  * [Adaptivity and Layout](#Adaptivity and Layout)

## <a name="UI Design Basics"/>UI Design Basics
### <a name="Designing for iOS"/>Designing for iOS
iOS包含了下面这些主旨：  
* `遵守`：UI帮助人们对内容进行理解和交互，而不是与其竞争。
* `清晰`：文本在每个尺寸都很清晰，图标是清晰且明白易懂的，装饰是巧妙而合适的，并且专注于使用的设计。
* `深度`：有层次感的视觉和合适的手势带来了活力，而且提升了人们的愉悦感和理解深度。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/1.png)  

无论你是在重新设计一个旧的app还是在创建一个新的app，考虑以下这些方法来处理工作：
* 首先，透过app的UI看到其核心功能并且确定它们的关联性。
* 然后，使用iOS的设计主旨使其充满于UI和用户体验。小心的添加细节和装饰，不要毫无理由地添加。
* 最后，确保你设计出的UI可以适应各种各样的设备和风格，这样你的用户可以在尽可能多的环境下享受你的app。

贯穿这个过程，准备好去打破常规、质疑设想，专注于内容和功能驱动每一个设计。

#### 服从内容
尽管一个清新的、漂亮的UI和流动的手势被iOS体验所强调，但用户的内容才是它的核心。  
这里是一些确保你的设计能够提升功能以及服从用户的内容的方法。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/2.png)

`利用全屏的优势。`天气app是这个方法的一个很好的例子：这个显示某个地区当前的天气的漂亮的、全屏的描述界面，包括那些显示每小时的天气信息的空间立即传达了最重要的信息。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/3.png)

`重新考虑物理的、真实的视觉指示物。`刃角、梯度和阴影效果有时会导致过重的UI元素，这会与内容竞争甚至压过内容。相反地，专注于内容，让UI扮演一个支持内容的角色。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/4.png)

`用半透明的UI元素暗示其后面的内容。`半透明元素——比如控制中心——提供了环境帮助用户看到有更多的内容是可获得的，并且可以给出一个短暂的信号。在iOS中，一个半透明的元素只在内容直接在其后方时变得模糊——给出一种透过米纸看的印象——它不会将屏幕的其余部分模糊化。

#### 指示清晰
指示清晰是另一个确保内容在你的app中占首要地位的方法。这里有一些方法可以使最重要的内容和功能变得清晰和易于交互。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/5.png)

`使用大量的负空间。`负空间可以使重要的内容和功能更加的明显和易于理解。负空间还会传达一种宁静的感觉，使app看上去更加的专注和有效。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/6.png)

`用颜色简化UI。`一个关键的颜色——比如便签中的黄色——强调了重要的信息并且不易察觉地指示了交互。它也给app带来一个持续的视觉主题。内置的app使用了一系列纯净的系统颜色，使其在各种色彩下以及黑暗或明亮的背景下都看起来不错。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/7.png)

`使用系统字体来确保清晰。`动态类型的San Francisco（一种iOS系统字体）可以自动地调整字母间距和行高，这样文本会易于阅读，在每个尺寸下都很好看。无论你使用San Francisco还是自定义的字体，确保使用动态类型，这样你的app可以在用户选择了不同的文本尺寸时做出响应。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/8.png)

`采取没有边界的按钮。`在默认情况下，所有的按钮都是无边界的。在内容区域，一个无边界的按钮通过上下文、颜色和一个呼唤操作的标题来表明交互。当它起作用时，一个内容区域的按钮可以展示一个稀薄的边界或者有颜色的背景来使其有差异。

#### 通过深度来传达
iOS通常在清晰的层级下展示内容来传达层级和位置，这可以帮助用户理解屏幕上各个物体的关系。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/9.png)

在一个支持3D Touch的设备上，轻按（peek）、重按（pop）和快速的响应动作使用户可以进入重要的功能或信息查看而不从运行环境中离开。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/10.png)

通过使用半透明的背景和在主屏幕上浮动出现，文件夹将自己的内容和屏幕上其余部分区分开来了。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/11.png)

提醒事件像所展示的那样在层级中显示了清单。当用户操作一个清单时，其余清单会一起收拢到屏幕的底部去。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/12.png)

日历在用户从年、月、日之间移动时通过增强的过渡效果给用户一种层次和深度的感觉。在这里展示的滚动年份视图中，用户可以直接看到今天的日期，还可以执行其他的日历任务。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/13.png)

当用户选择了一个月份，年份视图会放大推进然后显示月份视图。今天的日期依然高亮，年份则在返回按钮上显示，所以用户可以清楚的知道他们在哪个视图，从哪个视图来到这个视图的，以及如何回到原来的视图。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Designing%20for%20iOS/14.png)

当用户选择一个日期时会发生相似的过渡效果：月份视图会裂开，将当前一周的日期推到屏幕顶部，然后显示所选中日期的小时视图。通过每个过渡效果，日历加强了年份、月份和日期之间的层次关系。


### <a name="iOS App Anatomy"/>iOS App Anatomy
几乎所有的iOS app都至少使用了一些UIKit框架定义的UI部件。了解这些基础部件的名字、角色和功能可以帮助你明智地决定你的app的UI设计。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/iOS%20App%20Anatomy/1.png)

这些UIKit提供的UI元素大概分成四个种类：
* `Bars。`Bars包含可以告诉用户他们在哪的上下文信息和帮助用户导航或发起动作的控制装置。
* `Content Views。`Content Views包含app的详细内容，并且可以使用滚动、插入、删除和元件重布局的行为。
* `Controls。`Controls执行动作或者展示信息。
* `Temporary views。`Temporary views短暂地出现来给用户重要的信息或者额外的选项和功能。

除了定义UI元素以外，UIKit还定义实施功能的对象，比如手势识别、绘图、可及性和印刷支持。

从编程上来说，一个UI元素是一类视图（view），因为它继承自UIView。一个视图知道怎么在屏幕上绘制它自己，也知道用户在它的边界内触摸了它。控制器（比如按钮和滑动条）、内容视图（比如集合视图和表视图）和临时视图（比如警告框和选取器）都是视图的一种。

为了管理你app中的一系列视图，你最好使用视图控制器（View Controller）。视图控制器可以协调视图的显示，执行用户交互下的功能，还可以管理从一个到另一个屏幕的过渡。比如说，“设置”使用了一个导航控制器来显示他的一系列视图。

这个例子展示了视图和视图控制器是如何结合着呈现一个iOS app的UI的。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/iOS%20App%20Anatomy/2.png)

虽然开发者认为按照视图和视图控制器，用户趋于将一个iOS app当成一堆屏幕的集合去体验。从这个透视图看，一个屏幕（screen）广泛地符合一个app中清晰的视觉层次或者模型。

`NOTE`  
一个iOS app包含一个window。但是——不同于PC端应用的window——一个iOS window没有可见的部分，并且它不能移动到其他的位置。大部分的iOS app只包含一个window；支持额外的显示屏的app可以有多个window。

在《iOS Human Interface Guidelines》中，单词screen是大多数用户所理解的意思。作为一个开发者，你也许会在其他地方读到screen，比如UIScreen中的对象术语，你可以用其连接一个额外的显示屏。


### <a name="Adaptivity and Layout"/>Adaptivity and Layout
#### 构建自适应性
人们一般会想在他们所有的设备和多种环境下使用他们喜爱的app，比如不同的设备方向和iPad上的Splite View。尺寸的类和自动布局通过定义屏幕的布局、视图控制器和各个视图对于展示环境的改变做出的适应，来帮助你满足这一预期。（“展示环境”这一概念也涉及到时在整个屏幕显示和是屏幕的一部分去显示，比如弹出窗口（popover）的区域或者iPad上Splite View的一边区域。）

iOS中的显示环境由trait collection（iOS8引进的一个封装了Size Class等信息的新类）来定义，包括尺寸的类（size class）、显示比例和用户界面风格。你可以使用trait collection来使你的视图和视图控制器能够对显示环境的改变做出响应。（可以查看UITraitCollection Class Reference的开发文档来学习更多关于trait collection的内容。）

iOS定义了两个尺寸的类：regular（正常）和compact（紧凑）。regular尺寸类用于宽阔的空间而compact尺寸类用于紧凑的空间。你要设置一个水平尺寸类和一个垂直尺寸类来描绘一个显示环境。如你所想，一个iOS设备可以使用一系列的纵向尺寸类和另一系列的水平尺寸类。

iOS会在显示环境的尺寸类改变时自动地做出一系列布局改变。比如说，当垂直尺寸类从紧致变成正常，导航栏和工具栏会自动地去显示，比如弹出窗口（popover）的区域或者iPad上Splite View的一边区域。）

iOS定义了两个尺寸是如何描绘不同设备的显示环境的。比如iPad（包括iPad Pro）在所有尺寸和方向下都使用正常尺寸（regular）。换句话说，iPad的显示环境在水平和垂直上都是正常的尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/1.png)
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/2.png)

`NOTE`
在支持多任务处理的iPad上，你的app也许要和别的app共享屏幕。确保使用Auto Layout，这样你的app才会在用户决定使用多任务处理是进行响应，比如Splite View和SlideOver。
除了使用Auto Layout，当你在iPad Pro上展示可读的内容时使用UIView 的readableContentGuide属性也很重要，这可以使得边界对读者来说更加的舒适。

iPhone的显示环境非常依赖于设备和它的方向。

在垂直时，iPhone 6 Plus使用紧致的水平尺寸和正常的垂直尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/3.jpeg)

在水平时，iPhone 6 Plus使用正常的水平尺寸和紧致的垂直尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/4.jpeg)

在其他的iPhone机型上，包括iPhone 6，使用了同样的尺寸设置。

在垂直时，iPhone 6、iPhone 5和iPhone 4s使用紧致的水平尺寸和正常的垂直尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/5.jpeg)

在水平时，这些设备在水平和垂直尺寸上都是用紧致尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/6.jpeg)

#### 在各种环境下提供好的体验
使用自适应以后，你可以确保你的UI会对显示环境的改变进行适应。遵循这些指导方针来为用户提供一个在所有设备和环境下都优秀的体验。

`在所有环境下对主要内容保持关注。`这是最高优先项。用户使用你的app去查看和使用他们最关心的内容。当环境改变时UI也改变焦点的话，会使用户迷惑并且感觉丧失了控制。

`避免在布局上进行不必要的变动。`在所有环境下提供相似的体验可以让用户在旋转设备或者在其他设备使用app时保持一个相同的使用模式。比如说，如果你在水平正常的环境下使用网格来展示图片，当换成垂直紧致环境时，你不需要换成列表去展示相同的信息，即使你需要调整网格的尺寸。

`如果你的app只会运行在一个方向上，保持简单。`用户希望能在不同的方向上使用你的app，如果可能的话最好实现这个体验。但如果你必须让app只在一个方向上运行，你应该：
* `避免使用会提示用户旋转屏幕的UI元素。`在支持的方向上运行会清晰地告诉人们去旋转设备，如果一定要的话，不要添加不必要的杂乱的UI元素。
* `支持一个方向的所有形式。`比如说，如果一个app只支持水平方向，无论人们在持有设备时Home键是在左边还是右边，都应该可以正常使用。并且当人们在使用app时进行了180度的旋转，最好让内容也旋转180度来响应。

`当你的app在用户输入时会做出方向上的改变，使用app特有的方式来处理旋转。`比如说，一个通过旋转设备来移动游戏内容的游戏，是不能在屏幕旋转时做出旋转响应的。在这种情况下，你应该在所要求的不同方向下启动，然后允许用户在不同方向之间切换直到他们开始app的主任务。一旦用户开始主任务，就开始以app特有的方式来响应设备的移动。

#### 使用布局来表达
布局不仅仅只包括UI元素在app屏幕上的呈现。通过你的布局，可以让用户知道什么是最重要的，他们有哪些选择，以及事物是怎么关联的。

`通过增加重要的内容或功能的部分来使人们更加简单地专注于主要得任务。`一些好的方法是：将最重要的内容放在屏幕的上半部分——在左和右的选择上——靠近屏幕的左边：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/7.png)

`使用视觉的重心和均衡告诉用户屏幕上各个元素的相对重要性。`大的元素相比小的会更加吸引眼球和显得更加的重要。更大的元素也会让用户更加容易点击，让用户可以更加有效地使用——比如电话和时钟——那些用户经常在容易分心得情况下使用的内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/8.png)

`使用对齐方式来使浏览和与组件或层次的交互更加简单。`对齐方式使app看起来更整洁和有序，也会让用户在滚动屏幕查看信息时更加专注。不同信息组的缩进和对齐方式可以显示这些组的关系，并且可以让用户更加方便的找到关键信息。

`确保用户在默认尺寸下可以理解最主要得信息。`比如说，用户不应该需要横向滚动才能阅读重要的文本，也不应该需要放大才能看清主要得图片。

`准备好文本尺寸的更改。`用户希望大部分的app都能在他们从设置里选择了一个不同的文本尺寸后适当的进行响应。为了适应一些文本尺寸的更改，你也许需要调整布局；查看Text Should Always Be Legible来获取更多在app中展示文本的额信息。

`尽可能不要呈现不一致的UI。`一般来说，拥有相似功能的元素也应该看起来相似。人们认为他们注意到的不一致的地方一定有其原因，并且会花时间去弄明白这一点。

`给每一个交互的元素足够的空间来让人们易于与内容和控制器进行交互。`给可点击的控制器一个44*44像素的点击区域。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/9.png) ![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Adaptivity%20and%20Layout/10.png)
