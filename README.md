# iOS-Human-Interface-Guidelines
翻译苹果官方文档《iOS Human Interface Guidelines》

## 目录
* [UI Design Basics](#UI Design Basics)
  * [Designing for iOS](#Designing for iOS)
  * [iOS App Anatomy](#iOS App Anatomy)

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
