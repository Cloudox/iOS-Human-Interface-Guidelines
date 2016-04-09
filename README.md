# iOS-Human-Interface-Guidelines
翻译自苹果官方文档《iOS Human Interface Guidelines》

## <a name="Catalogue"/>目录
* [UI Design Basics](#UI Design Basics)
  * [Designing for iOS](#Designing for iOS)
  * [iOS App Anatomy](#iOS App Anatomy)
  * [Adaptivity and Layout](#Adaptivity and Layout)
  * [Starting and Stopping](#Starting and Stopping)
  * [Navigation](#Navigation)
  * [Modal Contexts](#Modal Contexts)
  * [Interactivity and Feedback](#Interactivity and Feedback)
  * [Animation](#Animation)
  * [Branding](#Branding)
  * [Color and Typography](#Color and Typography)
  * [Icons and Graphics](#Icons and Graphics)
  * [Terminology and Wording](#Terminology and Wording)
  * [Integrating with iOS](#Integrating with iOS)
* [Design Strategies](#Design Strategies)
  * [Design Principles](#Design Principles)
  * [From Concept to Product](#From Concept to Product)
  * [Case Study - From Desktop to iOS](#Case Study - From Desktop to iOS)
* [iOS Technologies](#iOS Technologies)
  * [3D Touch](#3D Touch)
  * [Live Photos](#Live Photos)
  * [Wallet](#Wallet)
  * [Apple Pay](#Apple Pay)
  * [Research Apps](#Research Apps)
  * [App Extensions](#App Extensions)
  * [HomeKit](#HomeKit)
  * [Multitasking](#Multitasking)
  * [Notifications](#Notifications)
  * [Social Media](#Social Media)
  * [iCloud](#iCloud)
  * [HealthKit](#HealthKit)
  * [In-App Purchase](#In-App Purchase)
  * [Game Center](#Game Center)
  * [iAd Rich Media Ads](#iAd Rich Media Ads)
  * [AirPrint](#AirPrint)
  * [Accessing User Data](#Accessing User Data)
  * [Quick Look](#Quick Look)
  * [Sound](#Sound)
  * [VoiceOver](#VoiceOver)
  * [Routing](#Routing)
  * [Edit Menu](#Edit Menu)
  * [Undo and Redo](#Undo and Redo)
  * [Keyboards and Input Views](#Keyboards and Input Views)
* [UI Elements](#UI Elements)
  * [Bars](#Bars)
  * [Content Views](#Content Views)
  * [Controls](#Controls)

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


### <a name="Starting and Stopping"/>Starting and Stopping
#### 立即开始
一般经常认为人们最多花一到两分钟时间来评估一个新的app。当你充分利用这段简短的时间立马展示有用的内容时，可以挑起新用户的兴趣并且给所有的用户一个超凡的体验。

`IMPORTANT`
不要告诉用户在安装你的app后重启设备。重启需要时间，而且会使你的app看上去不可靠以及难以使用。  
如果你的app有着内存使用或其他问题让其必须在系统刚启动时才能运行的话，你需要处理这些问题。查看Use Memory Efficiently获取一些开发一个优化的app的指导。

`尽可能地避免展示一个启动画面或者其他启动体验。`用户能立即使用的你的app是最好的。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Starting%20and%20Stopping/1.png) ![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Starting%20and%20Stopping/2.png)

`避免要求用户提供设置信息。`换成：
* `专注于80%的用户的需求。`当这样做时，大部分人们不需要去提供任何设置信息，因为app已经按照他们预期的来设置了。如果有功能只有一小部分用户需要——或者大部分用户只需要一次——舍弃它。
* `从其他来源获取尽可能多的信息。`如果你可以使用任何人们在安装app时提供的或者设备的设置中的信息，向系统查询这些值；不要要求人们再输入一遍。
* `如果你必须获取设置信息，提示人们在你的app内输入它们。`然后尽快存储这些信息（在你的app的设置里）。这样用户就不会在享受你的app之前被强制去切换到设置里。如果人们需要在之后修改这些信息，他们可以在任何时间去app的设置里改。

`尽可能地推迟登录的要求。`用户最好可以在没有登录的情况下进入你app的大部分界面并使用一些功能。比如说，App Store在用户决定要购买一些东西之前都不会要求用户登录。用户经常抛弃那些在他们没有使用任何功能前就强迫他们登录的app。

如果用户必须登录，在登录界面给出一个简短的、友好的解释说明登录的理由以及这能给他们带来什么好处。

`在提供启动页前小心的考虑。`（启动页介绍了一个app的功能以及解释如何执行一般的任务。）当你考虑启动页之前，尽力去设计你的app使其功能和任务都是直观而易于发现的。启动页并不是一个好的app设计的替代品。如果你仍然觉得启动页是必须的，遵循以下这些指导来创建一个简单的、目标明确的体验，而不妨碍到用户。

* `只给用户他们开始使用需要的信息。`一个好的启动页体验会告诉用户首先需要做些什么，或者简短地示范一些大部分用户感兴趣的功能。如果在用户有机会探索你的app之前给了太多的信息，会让你的用户觉得要记住一些他们暂时不需要的细节，并且会觉得你的app很难使用。如果在一些具体的任务上需要额外的帮助，只在用户执行这些任务时提供这些帮助。
* `使用动画和交互来吸引用户，并帮助他们在做中学。`只在文字能丰富体验时添加少量的文字；不要指望用户去阅读长篇大论。比如说，不要在可以用动画告诉用户如何使用时用文字去描述怎么执行的一个简单的任务。引导用户去执行一个更复杂的任务时，你可以添加一个短暂地的覆盖视图去简要地描述用户将要做的每一步。尽量避免使用app的截屏，因为他们不是交互式的而且用户会把他们和app的UI弄混。
* `让用户可以简单地去除或跳过启动页。`在用户看了启动页之后，他们也许不会想再看一次；还有一些用户也许根本就不想看到它。确保记住用户的选择并且不要让用户在每一次打开你的app时都再做一次。

`不要太早地要你的用户评价你的app。`太早地要求评价会打扰用户，也会降低得到的反馈的实用性。要鼓励深思熟虑的反馈，就要确保用户在你要求评价之前对你的app形成一个看法。比如说，你可以等到用户浏览了一个最低限度的不同界面的数量或者执行了一个最低限度的任务的数量再要求。

`一般来说，在设备当前的方向下启动。`不过，如果你的app只在一个方向上运行，你应该一直在那个方向上启动然后让用户旋转他们的设备。比如说，如果一个游戏或者视频app只在横向上运行，横向启动是最合适的，即使设备现在是垂直的。这样的话，如果用户在设备是垂直时启动app，他们就知道要旋转设备来查看内容了。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Starting%20and%20Stopping/3.png)

`NOTE`
一个只支持横向的app最好可以支持各种横向——就是说，Home键在左边或者在右边都可以。如果设备已经是横向的了，一个只支持横向的app应该在当前这个横向上启动，除非有很好的理由不这么做。否则，就在Home键在左边或者右边的横向都要能够启动。（查看Adaptivity and Layout来学习更多关于支持不同设备方向的内容。）

`提供一个启动文件。`iOS在你的app启动时展示一个图片——让你的用户觉得你的app很快，并能给你的app足够的时间去启动。查看Launch Files来学习如何创建一个启动文件。

`如果可能的话，避免要求用户在他们做任何其他事情之前去阅读一个免责声明或者同意一个终端用户许可协议。`你可以让App Store来展示你的免责声明或者终端用户许可协议（EULA），这样人们可以在他们获取到app之前访问这些内容。如果你必须在你的app内提供这些条目，确保让他们和你的UI和谐地融合在一起，并平衡好商业需求和用户体验的需求。

`当你的app重启时，修复它的状态这样用户就可以在他们退出的地方继续。`人们不应该要记住他们到达之前所在界面的步骤。查看Preserving Your App‘s Visual Appearance Across Launches来学习更多关于保护和修复你的app的状态的有效方式。

#### 永远准备停止
`一个iOS app从不提供一个关闭或退出选项。`人们会在切换到其他app、回到主屏幕或者让他们的设备进入睡眠模式时停止使用这个app。

当用户从你的app中切换出去时，iOS多任务处理器会将其过渡到后台去并且用新切换的app UI代替原有的UI。为这个情况做准备，你应该：
* `尽可能快的并以尽量合理的频率保存用户数据。`做这个是因为在后台的app会随时被告知退出或终止。
* `尽可能在停止时保存当前最好的细节状态。`这样做的话，人们在重新切回你的app时不会失去他们的使用环境。比如说，如果你的app展示滚动数据，保存当前滚动的位置。查看Preserving Your App‘s Visual Appearance Across Launches来学习更多关于保护和修复你的app的状态的有效方式。

一些app需要在用户前台运行其他app时保持在后台运行。比如说，用户会希望在他们使用一个app去检查他们的to-do列表或者玩一个游戏时，持续在另一个app中听歌。查看Multitasking来学习如何准确和得体地处理多任务。

`永远不要以编程的方式退出一个iOS app。`人们倾向于将这种情况视为闪退。如果某些东西因为功能问题阻止了你的app正常运行，你需要告诉用户这个情况并且解释他们可以为这个情况做些什么。这里有两个好方法：

`如果所有的app功能都无法获取，展示一个界面描述当前的状态并给出一些修复的建议。`这些信息可以给予用户反馈并让他们安心，说明你的app本身并没有出任何问题。这也可以让用户来控制，让他们决定是进行修复来继续使用你的app还是切换到其他的app。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Starting%20and%20Stopping/4.png)

`如果只有部分的app功能无法获取，当人们想要使用这个功能是显示一个界面或者一个警告框来告诉人们。`否则，人们可能会使用其他的app。如果你打算使用一个警告框，确保只在人们尝试获取无法获取的功能时才显示它。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Starting%20and%20Stopping/5.png)


### <a name="Navigation"/>Navigation
#### 导航栏
除非没有达到用户的期待，否则人们不会意识到一个app中导航栏的体验。你的工作就是在不引起注意的情况下，使用一种方式来实现导航栏来支持你app的结构和目的。

一般来说，有三种导航栏风格，每一种都很好的适应了一个独特的app结构：
* 层级
* 平面
* 内容或体验主导

在一个分层级的app中，用户通过在每一个屏幕做出一个选择来导航，直到到达了他们的目的地。为了导航到另一个目的地，用户必须回退一些步骤——或者从头开始——然后进行不同的选择。设置和邮件是使用分层结构的app的例子。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Navigation/1.jpeg)

在一个平面信息结构的app中，用户可以直接从一个基础分类导航到另一个基础分类，因为所有的基础分类都可以在主屏幕进入。音乐和应用商店是使用平面结构的app的例子。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Navigation/2.jpeg)

显然，在一个使用内容或体验导向的结构的app里，导航栏也是根据内容或体验来定义的。比如说，用户在书中直接从一页移动到另一页或者通过一个内容表单来选择页码；在一个游戏中，导航栏也经常是体验的一个重要部分。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Navigation/3.jpeg)

在一些例子中，将多个导航风格组合到一个app中会工作的很好。比如说，一个平面结构的某一个基础分类下的条目，使用层级结构来显示是最好的。

`用户也应该一直清楚他们在你的app的哪个位置，以及如何去往他们的目的地。`无论哪一种导航风格适合你的app，最重要的是，用户到达内容的路径是有逻辑的，可预知的，易于跟随的。

UIKit定义了一些基础的UI元素来简单的实现层级和平面导航风格，除了一些帮助你实现内容导向的导航栏元素，比如在一个图书风格或者多媒体浏览app中。一个提供体验导向导航风格的游戏或者其他app，通常依赖自定义的元素和行为。

`使用navigation bar来让用户简单的查看分层级的数据。`navigation bar的标题可以告诉用户他们现在在层级中的位置；返回按钮使回到之前的层级变得简单。查看Navagation Bar来学习更多。

`使用tab bar来显示对等的内容或功能类别。`tab bar是支持平面信息结构的好方法，并且可以让用户持续的在类别间切换，不管他们现在在哪个位置。查看Tab Bar学习更多。

`当每一个app的屏幕都表示同样类型的条目或页面的一个独立的实例时，使用page control。`page control可以很好地告诉用户有多少条目或页面是可接触的，以及现在显示的是哪一个。比如说，天气使用page control来显示用户打开过多少个地点的天气界面。查看Page Control学习更多。

`一般的，最好给用户一个可以到每个屏幕的路径。`如果有一个屏幕用户需要在多个环境下查看，考虑使用一个临时的界面，比如modal view、action sheet或alert。查看Modal View、Action Sheet和Alert学习更多。

UIKit还提供了如下这些相关的控制器：
* Segmented Control。segmented control让用户在屏幕在看到不同类别或方面的内容；它不能导航向一个新屏幕。
* Toolbar。即使toolbar看起来和navigation bar或tab bar很相似，它不能够导航。它只是给用户一些对当前屏幕内容动作的控制。


### <a name="Modal Contexts"/>Modal Contexts
Modality——即一种事物存在或体验的模式——优缺点并存。它可以让用户心无旁骛地完成任务或获取信息，但却是以临时性的禁止与app的其他内容交互来实现的。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Modal%20Contexts/1.png)

理论上，用户可以和iOS app非线性地交互，所以最好减少你app中模式化体验的数量。一般来说，只在下面这些情况下考虑模式化内容：
* 必须获取用户的关注时
* 一个独立的任务必须被完成——或者确定被抛弃——来避免在模糊不清的状态下丢失用户的数据。

`保持模式化任务简单、短暂和刚好被关注。`你不会想要用户将一个模式化界面当成你的app中一个迷你app来体验。如果一个子任务太复杂，人们会在进入模式化环境时忘记他们暂停的主任务。尤其在创建一个包含多层级视图的模式化任务时要谨慎，因为人们会迷失并忘记怎么回退回去。如果一个模式化任务必须包含多视图的子任务，确保给用户一个简单、清晰的路径来浏览层级，同时避免成环。查看Modal View来学习模式化界面。

`始终提供一个明显的、安全的方式来退出模式化任务。`人们应该能够预知他们退出一个模式化视图所带来的结果。

`如果任务需要一个多层级的模式化视图，确保你的用户理解他们按下一个顶层下面的视图的完成按钮时会发生什么。`检查任务来决定一个完成按钮是否只完成其自身界面的任务，还是整个任务。由于存在这种潜在的疑惑，尽量避免在次级的界面添加完成按钮。

`将警告框用于传达必要的——并且理论上可交互的——信息。`警告框会打断用户的体验并需要一次点击才能退出，所以让用户觉得这个警告框的信息是值得这次打断的。查看Alert学习更多。

`尊重用户接收通知的偏好。`在设置中，用户会指明他们希望如何从你的app中获取通知。确保遵守这些偏好，免得用户关闭你app的所有通知。


### <a name="Interactivity and Feedback"/>Interactivity and Feedback
#### 交互式的元素会引导触摸
为了显示交互，安装的app使用了一系列的提示，包括按压的相应、颜色、位置、环境和有意义的图标及标签。用户很少需要额外的装饰来告诉他们屏幕上的一个元素是可交互的或者说明它会做什么。

在一个支持3D Touch的设备上，当用户按压主屏幕上的一个图标时，他们看到的背景模糊表示了有更多的功能是可获取的。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/1.jpeg)

一个主颜色给用户一种很强的可交互的视觉暗示，特别是在那些不使用丰富的其他颜色的app中。在通讯录中，蓝色标志了可交互元素，并给app一种统一的，可辨识的视觉主题。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/2.jpeg)

这个返回按钮使用了很多的提示来表示它的可交互性，并传达它的功能：它在导航栏中出现，它显示了一个返回的V形标记，它典型地使用了一个主颜色，并且它显示了一个标题来描述上一个屏幕。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/3.jpeg)

一个提供了明确的动作响应的图标或标题会吸引用户来点击。比如说，地图中的标题，例如“Flyover Tour”和“Directions to Here”明确的描述了用户会执行的动作。结合一个主颜色，可执行的标题会使用按钮边界或其他多余的装饰。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/4.jpeg)

`在一个内容区域，只在需要时添加按钮边界或者背景。`在bars、action sheets和alerts中，因为用户知道这些区域中的大部分元素都是可以交互的，所以不需要边界。另一方面，在一个内容区域中的按钮就需要一个边界或者背景来区分它和内容的其他区域。比如说，音乐、时钟、照片和App Store就在一些特殊的环境下使用这样的按钮。

照片使用了按钮边框来区分Start Sharing按钮和它上面的解释文字。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/5.jpeg)

时钟在计时器和Timer屏幕中使用了按钮背景来将人们的注意力吸引到Start和Pause按钮上，使人们即使周围的环境很分散注意力也能容易的点击到按钮。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/6.jpeg)

App Store在列表行中使用按钮边框来强调点击行获取更多信息和点击按钮来开始（或安装）一个购买的区别。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/7.jpeg)

#### 用户知道标准的手势
用户使用手势——例如点击、拖拽和收缩——去和apps以及iOS设备交互。使用手势给了人们一个和设备的近距离沟通，并且加强了对屏幕上物体的直接操纵感。人们希望他们使用的所有app中手势都是同样工作的。

人们不需要为了使用3D Touch而学习新的手势。当人们轻按屏幕得到响应的时候，会很快发现3D Touch带来的新的交互维度。

`Tap（点击）：`按或选择一个控制器或元素

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/8.jpeg)

`Drag（拖拽）：`去滚动或摇——即左右摇摆。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/9.jpeg)

`Flick（轻弹）：`快速的滚动或摇。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/10.jpeg)

`Swipe（滑动）：`用一个手指，来回到上一个界面，或在一个分裂视图控制器中显示一个隐藏的界面，或者是显示列表行中的删除按钮。使用peek，滑动可以显示快速响应的内容（查看3D Touch来获取更多信息）。
使用四个手指，在iPad上切换app。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/11.jpeg)

`Double tap（双击）：`放大并居中内容中的一块区域或图片。
如果已经放大了，则是缩小。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/12.jpeg)

`Pinch（捏）：`外捏来放大；内捏来缩小。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/13.jpeg)

`Touch and hold（触摸并保持）：`在可编辑或可选择的文本区域，展示一个光标位置的放大的视图。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/14.jpeg)

`Shake（摇晃）：`来开始一个撤销或重复的动作。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/15.jpeg)

除了用户知道的标准手势，iOS还定义了一些唤起全系统动作的手势，比如显示控制中心或通知中心。无论人们使用什么app，都依赖于这些手势去操作。

`不要给标准手势关联不同的动作。`除非你的app是一个游戏，重定义一个标准手势的意义会使你的用户感到困惑并使你的app变得难用。

`不要自定义会调用标准手势相同动作的手势。`人们习惯标准手势的行为，而且他们并不会对学习不同的方式来做同样的事情感到感谢。

`使用复杂的手势作为加快任务的快捷方式，而不是完成它的唯一方式。`尽可能地给用户一个简单、直接的方式来完成动作，即使这需要额外的一两次点击。简单的手势让用户集中在体验和内容上，而不是交互。

`一般来说，不要定义新的手势，除非你的app是个游戏。`在游戏或其他沉浸式app中，自定义的手势会变成有趣体验的一部分。但对于一些帮助用户做一些对他们来说重要的事情的时候，最好使用标准手势，因为用户不需要努力去发现或记住他们。

`在一个合理的环境下，考虑使用多触点的手势。`尽管复杂的手势在每一个app中都不被期待，它们却可以丰富app的体验，使人们在其中度过大量的时间，比如在游戏或创造内容的环境下。永远记住，非标准手势不是可发现的，并且应该稀少，如果有，那么就要是完成动作的唯一方式。

#### 反馈帮助理解
反馈帮助人们知道一个app正在干什么，发现他们接下来可以做什么，并理解他们动作的结果。UIKit的控制器和视图提供了很多种反馈。

`尽可能地整体化常规的和其他相关的反馈信息到你的UI中。`最好用户可以不需要动作就获取这种类型的信息，并且不会被他们的内容迷惑。比如说，邮件在工具栏显示了当前信箱的状态，这样就不会和用户的内容竞争。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/16.jpeg)

`避免不必要的警告框。`警告框是一种很有力的反馈机制，但它只应该用于显示重要的——并且情理上可交互的——信息。如果用户看到了太多包含不重要信息的警告框，他们很快会变得忽略所有的警告框。查看Alert学习更过关于警告框的使用。

#### 输入信息应该简单
不论用户是点击控制器还是使用键盘，输入信息都花费时间和注意力。当一个app在展现有用的内容之前因为要求太多用户输入使人们进度变慢，人们会对使用它变得气馁。

`让用户做选择变得简单。`比如说，你可以使用一个选择器或列表代替文本框，因为大多数用户认为从列表中选择一个元素比输入文字要容易。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Interactivity%20and%20Feedback/17.jpeg)

`合适的从iOS获取信息。`用户在他们的设备中存储了大量的信息。可以的话，不要强制用户给你一些你可以很容易自己找到的信息，比如他们的联系人或日历信息。

`通过给用户一些有用的内容来平衡输入的请求。`给予和获取的感受帮助人们感觉他们在你的app中正在前进。

### <a name="Animation"/>Animation
#### 动画
漂亮、精细的动画贯穿了iOS 的UI，并且使app的体验变得更加的迷人而有活力。
恰当的动画可以：
* 传达状态和提供反馈
* 增强操纵的直接观感
* 帮助人们显示他们操作的结果

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Animation/1.jpeg)

`慎重地添加动画，特别是在那些非沉浸式体验的app里。`过多无用的动画会妨碍app的流程，降低性能，并使用户从他们的任务中分心。

特别是要使用运动效果和UIKit动态行为为目的和约束，并确保测试结果。使用合适的话，这些效果可以提升用户的理解和享受过程；过度使用它们则会使app看起来迷惑和难以操控。

`合适的时候，使自定义的动画和内嵌的动画保持一致。`用户习惯了内嵌在iOS app中精细的动画。事实上，用户倾向于将视图间平滑的过渡、改变设备方向时流动的响应、和符合物理原理的滚动作为对iOS体验的期待。除非你正在创造一个沉浸式体验的app——譬如游戏——否则自定义的动画应该和内嵌的动画保持一致。

`让动画始终贯穿你的app。`就如其他类型的定制化一样，始终使用自定义动画来贯穿很重要，这样用户就会从使用你的app中建立体验。

`一般来说，在自定义动画中追求现实性和可信性。`用户倾向于期望获取艺术性的外表，但是他们会在体验无意义或无视物理规律的运动时感到迷惑。比如说，如果你从屏幕的顶端滑动到底部来展现一个视图，你应该在销毁这个界面时让它原路返回，这样可以帮助用户记住视图是从哪来的。如果你继续往下滑动来销毁这个视图，你就打破了用户对其从屏幕顶端出现的心理模型。

### <a name="Branding"/>Branding
#### 品牌推广

成功的推广不仅仅是在app中添加品牌资源。最好的app会将已有的资源整合在统一的视觉里，并且会给用户一种愉悦的、难忘的体验。

iOS可以非常简单的使用自定义的图标、颜色和字体来创造一个与众不同的UI，使你的app区别于其他的app。当你设计这些元素时，牢记两件事：
* 每个自定义的元素自己都应该好看且功能良好，但是它也应该看起来和app中的其他元素统一，不论它们是自定义的还是标准的。
* 要在iOS中宾至如归，app不需要看起来像内置的app，但需要在遵守、清晰、深度上统一（查看[Designing for iOS](#Designing for iOS)学习更多关于这些主旨的内容）。花时间思考在你的app中遵守、清晰、深度意味着什么，然后在自定义的元素中表达出来。

如果你需要在你的app中提示用户一个现有的品牌，遵守以下这些指南。

`精妙、不唐突的包含品牌资源。`人们使用你的app来做事情或者娱乐；他们不想感觉到他们被强制观看一段广告。最好的用户体验是，安静的从你选择的字体、颜色和图像中提示用户品牌本身。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Branding/1.jpeg)

`不要占用人们关心的内容区域。`比如说，在屏幕顶端显示一个持久的第二显示栏，除了展示品牌资源外不做任何事情，这意味着内容区域变少了。相反，尊重用户的内容并且考虑少使用打扰的方式展示无处不在的广告，比如使用一个自定义的色调或字体，或者巧妙地自定义屏幕背景。

`抵制贯穿于app地展示你的logo的诱惑。`移动设备的屏幕相对较小，每一次logo的出现都会占据用户想要看到的内容空间。并且，在app中显示logo并不会达到在web页面里显示的同样目的：用户打开一个未知的web页面很普遍，但用户打开一个iOS app之前通常都会看app的图标。

### <a name="Color and Typography"/>Color and Typography
#### 颜色和排版
#### 颜色增强沟通
在iOS中，颜色帮助指明交互、给予活力、并提供视觉连贯性。内置的app使用了一系列无论从个体上还是整体上看，或者明亮和阴暗的背景下看都很棒的纯净的颜色。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Color%20and%20Typography/1.jpeg)

`如果你创造了多种自定义颜色，确保他们整体效果良好。`比如说，如果蜡笔在你的app风格中是必须的，你需要创造一系列协调的蜡笔色贯穿你的app。

`关注颜色在不同环境中的对比。`比如说，如果导航栏背景和栏上的按钮标题没有对比度，用户就很难看到这些按钮。一个快速但不科学的检验你的颜色是否有足够的对比度的方法是：在一个不同亮度下的设备上查看你的app，包括太阳天的户外环境。

即使在设备上查看你的app可以帮助你找到一些你需要调整的区域，这仍然取代不了更加客观地得出可靠结果的方式。这种方法包括测定前景和背景颜色亮度的比值。你可以使用在线对比比值计算器或者自己使用符合WCAG 2.0标准的公式来计算去获取这个比值。app中理想的颜色对比值为4.5:1或更高。

`当你使用自定义的栏色调时考虑半透明的栏和app内容。`如果你需要创造一个匹配特殊颜色的栏色调，比如一个商标中的颜色，你也许需要尝试很多种颜色才能得到想要的结果。一个栏的外观会被iOS提供的半透明效果和app中在栏后方出现的内容共同影响。

`API NOTE`
使用tintColor属性来设置栏上按钮标题的色调；使用barTintColor属性来设置栏本身的色调。查看UINavigationBar Class Reference，UITabBar Class Reference，UIToolbar Class Reference，和UISearchBar Class Reference来学习更多关于栏的属性。

`注意色盲。`大部分色盲患者难以区分红色和绿色。测试你的app确保没有任何地方使用红色和绿色作为唯一区分两种状态和值的方式（一些图片编辑软件有工具可以帮助你校验色盲）。一般来说，使用多种方式来显示一个元素的交互是好的方法（查看Interactive Elements Invite Touch学习在iOS中显示交互的内容）。

`考虑选择一个主颜色来显示交互和状态。`内置的app中的主颜色有备忘录中的黄色和日历中的红色。如果你确定一个主颜色去显示交互和状态，确保app中的其他颜色不与其竞争。

`避免对可交互和不可交互的元素使用相同的颜色。`颜色是UI元素表示其是否可交互的一种方式。如果可交互和不可交互的元素有了相同的颜色，用户很难知道点击那里。

`颜色会沟通，但并不总是你想要的方式。`每个人看待颜色都不一样，很多文化也对颜色的意义有不同的定义。花时间去研究你使用的颜色在其他的国家和文化中会被怎样感知。你会想要尽可能地确保你app中的颜色传达合适的信息。

`大部分情况下，不要让颜色使用户分心。`除非颜色是你app的必要目的，否则让颜色成为一种微妙的优化方式。

#### 好的排版使沟通更清晰
苹果设计了San Francisco系列排版来提供一种贯穿全平台的漂亮的、一致的声音和阅读体验，在iOS 9 之后，San Francisco变成了系统字体。

San Francisco与动态排版（Dynamic Type）携手工作来给你：
* 在所有用户设置中一系列的自动字体尺寸，包括无障碍设置中提供了最高的识别率的和很好的的阅读体验
* 每一种字体尺寸都自动调节字母间距（字距）和行高
* 能够为语义不同的文本块指定不同的文本风格，比如正文、注脚和标题
* 对用户做出的文字大小设置进行合适的响应变化（包括无障碍的文字尺寸）

访问[https://developer.apple.com/fonts/](https://developer.apple.com/fonts/)下载San Francisco。（注意iOS 9 中San Francisco字体叫SF-UI）当你在你的app中采用San Francisco时，你可以在模拟器 > 设置中调整数值来测试你的app文本在不同尺寸下的表现。

`NOTE`
如果你使用自定义的字体，仍然可以根据系统设置中的的文本尺寸调整动态排版和比例类型。你的app要对用户改变设置时做出适当的响应。查看Text Styles来学习如何使用文本类型在用户改变文本尺寸设置时确保app得到通知。

San Francisco包括两种视觉尺寸：Text和Display。Text用于低于20点的尺寸，Display用于高于20点的尺寸。当你在你的app中使用San Francisco时，iOS会自动地在Text和Display中切换。

`NOTE`
如果你使用类似Sketch或Photoshop的应用来创建你的设计，你需要在设置20点以上的类型时切换到Display。iOS会自动地为San Francisco调整建立在字体尺寸上的跟踪值（Tracking value）（跟踪值用来修改某个点尺寸下的字母间距）。Text和Display中每个尺寸的跟踪值分别显示在表10-1和表10-2中。

表10-1 在SF-UI Text中每个尺寸的跟踪值  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Color%20and%20Typography/2.jpeg)

表10-2 Display中每个尺寸的跟踪值  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Color%20and%20Typography/3.jpeg)

为了强调某些文本或者创造不同内容部分之间的视觉关系，你可以依靠动态排版支持的语义定义样式，比如标题和正文，或者指定字体宽度，比如纤细和半粗。采用动态排版风格可以简单地传达你内容的意义，但是如果你想要更多对设计的掌控，你也可以对某个特定的文本块设置特定的宽度。（查看UIFont Class Reference学习更多关于调整文本宽度的内容。）

比如说，你也许会想要增加某个文本的宽度来帮助用户了解内容的层级或者吸引他们的注意力到某个特定的单词或短语。或者你想要增加小字体的宽度并减小大字体的宽度来创造一种多个靠近的文本的凝聚感。字体宽度对整体风格和内容表达也具有显著的影响，所以你也许会选择一个特殊的宽度来达到一种特殊的设计目标。

`当响应文本尺寸变化时区分优先次序。`不同内容对用户的重要性是不同的。当用户选择一种更大的文本尺寸时，他们是想要让他们关心的内容更加易于阅读；他们并不想让屏幕上的每一个单词都变得更大。

比如说，当用户选择一个大的无障碍文本尺寸，邮件会将标题和文本用大的尺寸显示，但不会变化其他重要的文本——比如日期和收件人。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Color%20and%20Typography/4.jpeg)

`确保自定义字体在每一种风格、不同的尺寸下都是清晰的。`方法是对iOS在不同尺寸下显示不同字体风格的方式进行模仿。比如：
* 文本永远不应该小于11点，即使用户选择了特小号的尺寸。相应的，正文风格使用17点作为默认的大尺寸。
* 一般来说，在每种尺寸设置下，字体尺寸和引导值相差一点。只有两种标题风格例外，它们在特小号、小号和中号下使用相同的字体尺寸、引导值、跟踪值。
* 在最小的三种文本尺寸下，跟踪值会相对地大一些；在最大的三种文本尺寸下，跟踪值会相对地紧致一些。
* 标题和正文风格使用相同的字体尺寸。为了区分正文风格，标题使用了更宽的宽度。
* 导航栏中的文本使用17点，与正文风格在大号下相同。
* 文本总是使用常规或中号宽度；它不使用浅或粗体，因为浅和粗体在小号下看起来不好。

`一般来说，在你的app中使用单一的字体。`混合多种不同的字体会使你的app看起来零散和稀松。相反的，要使用一种字体以及少量的风格和尺寸。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Color%20and%20Typography/5.jpeg)

### <a name="Icons and Graphics"/>Icons and Graphics
#### App图标
每个app都需要一个漂亮的app图标。人们经常会根据你的app图标生成对你app的第一印象，包括你app的质量、目的和可靠性。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Icons%20and%20Graphics/1.jpeg)

当你思考你的app图标时，考虑下面这些事情。当你准备去创建它时，查看App Icon获得更多的指导和规格。
* app图标是你app品牌很重要的一部分。将设计作为一个讲述你app故事的机会，并建立和用户之间的情感沟通。
* 最好的app图标是独特的、整洁的、迷人的并且难忘的。
* app图标需要在不同尺寸下和不同背景下都看起来不错。在大尺寸在丰富图标的细节可能会在小尺寸下模糊不清。

#### 小图标
iOS提供了很多的小图标——表示常见的任务和内容类型——给标签栏、工具栏、导航栏和主页面快速访问使用。尽可能多的使用内置图标是一个好主意，因为用户已经知道他们代表什么意思了。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Icons%20and%20Graphics/2.jpeg)

如果你需要表示自定义的动作和内容类型，你可以创造自定义的栏图标。设计这些小的、精简的图标和设计app图标是非常不同的。如果你需要创造一个自定义的栏图标，查看Template Icons学习怎样创造。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Icons%20and%20Graphics/3.jpeg)

注意那些在导航栏或者工具栏中可以使用文字代替图标表示条目的地方。比如说，日历在工具栏中使用了“Today”、“Calendars”和“Inbox”代替图标。

考虑屏幕上一次可以看到多少图标，来帮助你决定在你app的导航栏或工具栏中你是应该使用文字还是图标。在一个屏幕上使用太多图标会让app看起来难以编译。还有，注意当在横向环境时这个决定也许会不同，因为横向环境会有更多的空间在栏上显示文字。

#### 图形
iOS app往往生动丰富。无论你是在展示用户的图片还是创造一个自定义的插图，都应该遵守下面这些指南。

`支持视网膜（Retina）显示。`确保你提供了你app中所有插图和图形的高分辨率资源。尤其是，为iPhone 6 Plus提供@3x资源，为其他所有高分辨率设备提供@2x资源。

`在原始长宽比上显示照片和图形，并避免拉伸超过100%。`你不希望你app中的插图和图形看起来倾斜和太大。让用户选择他们是否要放大或缩小图片。

`不要在你的设计中使用复制苹果产品的图片。`这些标志是受版权保护的，并且产品的设计常常会改变。

`不要在你的设计中使用苹果的app图标、图片和截屏。`苹果的设计是受版权保护的，除非他们是系统提供的，否则不能出现在你的UI中。

### <a name="Terminology and Wording"/>Terminology and Wording
#### 术语和词汇
每一个你显示在app中的单词都是你和用户交流的一部分。利用这个交流的机会来让用户觉得清晰并帮助用户在你的app中感到舒适。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Terminology%20and%20Wording/1.jpeg)

设置对每个用户来说都是基本且必要的，所以他使用了简单、直接的语言告诉用户可以做什么。比如说，设置（Settings）>免打扰（Do not Disturb）解释了很多选项的效果，而没有使用一些可能会让纯朴的用户不能理解的术语。

`使用你确保你的用户能理解的术语。`根据你对用户的了解来确定你打算使用的单词和短语是否合适。比如说，在面向纯朴用户的app中技术术语没有任何帮助，但是对于为理解技术的用户设计的app则很合适。

`使用非正式并友好的语气，但不要太随意。`你会想避免呆板和太正式，但是你不会想要冒听起来快乐到虚伪或傲慢的险。记住用户可能在你的UI中阅读文本很多次，那些第一次看觉得机智的内容重复看的时候可能会变得刺激人。

`像一个新闻编辑一样思考，并提防多余或不必要的单词。`当你的UI文本短而直接时，用户会很快很容易的理解。确定最重要的信息，简明的表述它，然后显著地显示它，这样用户就不用阅读大量的文字找到他们要找的或者了解他们接下去该做什么。

`给控件赋予简短的文字或者使用易理解的图标。`人们应该看一眼就能知道一个控件是做什么的。

`描述日期时注意精确。`大多时候，在你的UI中使用友好的词语比如今天和明天来显示日期信息是合适的。但是当你没有计算用户当前的位置时可能会变得迷惑。比如说，有一件事恰好在午夜前开始，对于同一个时区的用户来说，这件事是今天开始的，但对于早一些时区的用户来说，同一件事可能是昨天开始的。

`编辑一段好的App Store描述来尽可能的多和潜在的用户交流。`除了精准的描述你的app以及对你认为人们最感兴趣的品质进行高亮以外，确保：
* `纠正所有的拼写、语法和标点符号错误。`尽管这种错误不会影响每个人，对有些人来说这会带来一种对你app质量的坏印象。
* `保持全大写单词在一个最小的数量。`有时候全大写单词可以吸引人们的注意，但当整段话都是大写的时候，它会很难阅读而且会看起来像叫喊。
* `考虑描述特殊的bug修复。`如果你app的新版本包含了用户期望的bug修复，最好在描述中提到它。

### <a name="Integrating with iOS"/>Integrating with iOS
#### 和iOS整合
和iOS整合的意思是给用户一种吸引人的、愉快的体验来让用户在平台上宾至如归；它不是说要创建一个看起来像复制内置的app一样的app。

将你的独特的app和平台整合的最好方式是理解促进iOS的那些主旨——在[Designing for iOS](#Designing for iOS)中有这些主旨的描述——并且思考你的app怎样表达它们。为了达成这个目标，遵守这一节的指南可以帮助你给予用户他们期待的体验。

#### 恰当的使用标准UI元素
尽可能的使用UIKit提供的标准UI元素是好的方式。当你使用标准元素而不是自定义一个时，你和你的用户都可以获益：
* 标准UI元素会在iOS提供重新设计的样式时自动获取更新——自定义的元素不会获取更新。
* 标准UI元素会提供很多种自定义他们样式或行为的方式。比如说，所有的视图（即继承自UIVies的对象）都可以使用tintColor属性进行上色，这就可以很容易的为你的app加上颜色。
* 人们会对标准UI元素感到习惯，所以他们可以很容易的理解怎样在你的app中使用它们。

为了得到这些使用标准UI元素带来的优势，这些事情很重要：

`遵守每一个UI元素的指导方针。`当一个UI元素看起来和工作起来都符合人们期待的方式的时候，人们就可以根据以前的经验来帮助他们在你的app中使用它。你可以在Bars、Content Views、Controls和Temporary Views中找到UI元素的指导方针。

`不要混合不同iOS版本下的UI元素风格。`你不会希望通过显示看起来像在不同于当前设备运行的iOS系统版本的UI元素来让用户感到迷惑。

`一般来说，不要创建一个自定义的UI元素来展现标准的动作。`首先，问问你自己为什么你要创建一个行为和标准UI元素一样的自定义UI元素。如果你只是想要一个自定义的外表，考虑使用UIKit的外表定制API来改变一个标准元素的外观，或者上色。如果你想要一些稍微不同的行为，确定找出一个标准元素在调整性能和属性后会不会做出你想要的效果。如果你需要完全自定义行为，最好设计一个看起来不那么像标准元素的自定义元素。

`TIP`
Interface Builder让获取标准UI元素，使用外观定制API，修改性能和属性，以及为你的控件使用自定义和系统提供的图标变得很容易。查看Xcode Overview学习更多关于Interface Builder的内容。

`不要使用系统定制的按钮和图标来表示其他东西。`iOS提供了很多你可以用在你app中的按钮和图标。确保你理解了文件上记录的这些按钮和图标的含义；不要依赖于你对他们外表的理解。（你可以在Toolbar and Navigation Bar Buttons和Tab Bar Icons中找到每个图标的含义。）

如果你不能找到一个系统提供的按钮或图标来合适的表述你app中的一个功能，你可以创建你自己的。查看Bar Button Icons来获取指导方针帮助你设计自定义图标。

如果你的app提供了沉浸式的任务或体验，创建完全自定义的控件就变得有意义。这是因为你在创建一个独特的环境，探寻如何去控制这个环境是用户在这种app中所期待的体验。

#### 淡化文件和文档处理
iOS app可以帮助人们创建和操作文件，但这不意味着人们需要思考iOS设备上的文件系统。

如果你的app帮助人们创建和操作文档，最好提供一些app独特的文档库视图来让用户打开一个已有的文档或者创建一个新的文档。理论上，这种库应该：
* `是高度图形化的。`人们应该能够可以通过屏幕上的文档视觉呈现来简单的鉴别他们想要的文档。
* `让人们通过最少的手势来做他们想做的。`比如说，人们可以水平的滚动一个已存在文档组成的滚轮或者网格来找到他们想要的文档，并通过一次点击打开它。
* `包含新建文档的功能。`一个文档库应该可以通过点击一个图标来创建一个新的文档，而不是让人们到别的地方去创建新的文档。

比如说，Pages通过一个图形化的文档库视图和一个简单的创建新文档的方式来展示用户的文档。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Design%20Basics/Integrating%20with%20iOS/1.jpeg)

`TIP`
你可以使用快速预览特性来让人们在你的app中预览文档，即使你的app不能打开他们。查看Quick Look来学习怎样在你的app中提供这个特性。

如果你的app允许人们使用他们在别的app中创建的文档，你可以显示一个文档选取控制器来帮助他们使用这些文档。文档选取控制器可以显示那些存在用户iCloud Drive中的除了Document Provider extensions中的文档，这与其他创建文档或者存储文档的app相关联。查看Document Provider Extensions学习更多关于Document Provider extensions的内容；查看Document Picker Programming Guide学习更多关于文档选取控制器的内容。

`给人们他们的工作始终都被保存的自信，除非他们明确的取消或删除它。`如果你的app帮助人们创建或者编辑文档，不要要求他们进行明确的存储动作。iOS app应该为存储用户的输入负责，包括周期地和他们打开其他的文档或在app间切换的时候。

如果你app的主要功能不是创造内容——但你允许人们在查看信息和编辑信息之间切换——要求他们保存更改就变得有意义。在这种情况下，最好在查看信息的界面提供一个编辑按钮。当人们点击编辑按钮时，用保存按钮代替它并添加一个取消按钮。编辑按钮的转变提醒人们他们是在编辑模式，并且也许需要保存更改，而取消按钮让他们可以不保存更改的退出。

#### 如果必要的话，实现可配置
一些app也许需要给用户设置或配置选项的方式，但大多数app可以避免或延后这个工作。成功的app适应大多数人，当然也提供一些便捷的方式去调整用户体验。

当你以大部分用户期待的方式设计你的app时，你就降低了设置的需求。如果你需要用户的信息，向系统寻求而不是要求用户来提供。如果你认为以一定要提供人们很少会改变的app设置，查看The Setting Bundle来学习怎样在你的代码中支持它们。

`尽可能的，在主UI中提供配置选项。`当该选项是主任务并且人们经常会想要改变它们的时候，将其放在主UI就会有意义。如果人们只是偶尔改变app的配置，就将其放在分页面。

`必要的话，帮助人们直接在设置中去到你app的设置。`尤其是如果你显示一段描述如何找到你的设置的信息，比如“去往设置>我的app>隐私>定位服务”，用一个直接去往这个位置的按钮代替描述。查看Setting Launch URL学习如何实现这个动作。

#### 利用iOS技术
iOS提供了丰富的技术来用用户期待的方式支持常见的任务和情景。这个期待意味着，将系统支持的技术整合进你的app总是会比设计一个自定义的方式要好。

一些iOS技术——比如Multitasking和VoiceOver——是所有app都应该包含的系统特性。其他的可以实现特殊的app功能，比如处理票和礼物卡片（Wallet），让用户使用app购买（In-App Purchase），展示app内置广告（iAd Rich Media Ads），结合Game Center以及支持iCloud。

## <a name="Design Strategies"/>Design Strategies
### <a name="Design Principles"/>Design Principles
#### 设计原则
#### 整体美学
整体美学并不是测量一个app插图的美丽程度或者表述它的风格；而是表示一个app的外表和行为与其功能整合来传达一种连贯的信息的程度。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Design%20Principles/1.jpeg)

人们关心一个app是否提供了它承诺的功能，但同时也受到app的外表和行为的很大——有时是潜意识的——影响。比如说，一个帮助人们完成严肃任务的app会通过将装饰性的元素做的精妙且不引人注目和使用标准控件以及可预见的行为来将注意力集中到任务上来。这个app传达了一个关于其目的和身份的清晰的、统一的信息来帮助人们信任它。但如果这个app通过在干扰的、轻浮的、随意的UI中展现任务来传递混乱的信号，人们就会对app的可靠性和可信度产生疑问。

另一方面，在鼓励沉浸式体验的app中——比如游戏——人们会期待迷人的外表，这会带来愉悦、轻松的感受并鼓励探索。人们不会期待在游戏中完成严肃的或生产性的任务，但是他们会期待游戏的外表和行为与其目的相整合。

#### 一致性
一致性让人们可以在一个app的不同部分的UI间或不同app之间传递他们的知识和技能。一个一致性的app不是盲目的复制其他app，也不是在文本上停滞不前；而是关注标准和典型的人们所期望的东西并提供一种内在的一致体验。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Design%20Principles/2.jpeg)

思考这些问题来确定一个iOS app是否遵循了一致性的原则：
* app是否和iOS的标准一致？它是否正确地使用了系统提供的控制器、视图和图标？它是否以用户所期待的方式包含了设备的特性？
* app其自身是否一致？文本是否使用了同样的术语和风格？同样的图标是否总是表示同样的事情？人们是否能预测在不同地方执行相同操作时产生的结果？自定义的UI元素在整个app中的外表和行为是否一致？
* 同样的，app是否和其早期的版本一致？术语和意义是否保持一致？基本的概念和基础的功能是否在本质上没有改变？

#### 直接操控
当人们直接操控屏幕上的对象而不是使用单独的控件来操控它们时，他们会更加专注于他们的任务，也会更容易理解他们的动作所带来的结果。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Design%20Principles/3.jpeg)

使用多点触控界面，人们可以通过捏来直接展开或收缩一个图像或内容区域。在游戏中，玩家通过屏幕上的对象来直接移动或互动——比如说，一个游戏也许会展示一个用户能够通过旋转打开的锁。

在iOS app中，人们会在这些时候体验直接操控：
* 旋转或移动设备来影响屏幕上的物体
* 使用手势来操控屏幕上的物体
* 能够看见他们的动作有即时的、可见的结果

#### 反馈
反馈可以确认人们的动作，给他们展示结果，并更新他们任务的进展。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Design%20Principles/4.jpeg)

内置的iOS app为每一个用户动作提供了可感知的反馈。列表元素和控制器会在人们点击时简短的高亮并且——在操作持续几秒钟后——控制器会显示进展。

精细的动画会给予人们有意义的反馈来帮助弄清楚他们动作的结果。比如说，列表会在添加一行时显示动画来帮助人们看到变化。

声音也可以给人们有用的反馈，但这不应该是唯一的反馈机制，因为人们不会永远听到他们设备的声音。

#### 象征
当一个app中虚拟的对象和操作象征着熟悉的经验时——无论这些经验是基于现实世界还是数字世界——用户会很快理解如何使用app。

一个app最好使用那些不会局限于他们所基于的对象或操作的象征来支持使用或经验。

iOS app有着非常大适用范围的象征，因为人们在直接和屏幕交互。iOS中的象征包括：
* 移动分层视图来露出他们下方的内容
* 在游戏中拖拽、轻拂或猛击物体
* 点击开关、滑动滚动条和旋转选取器
* 轻拂来在书或杂志中切换页面

#### 用户控制
人——而不是app——才应该发起和控制操作。app可以建议一个操作过程或者警告危险的后果，但app从用户手中夺走决定权通常是错误的。最好的app会在给予人们他们想要的能力和帮助人们避免不想要的结果中找到准确的平衡。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Design%20Principles/5.jpeg)

当行为和控制是相似的且可预测的时，用户会感到更多的对一个app的控制力。而当操作是简单和直接的时，用户会很容易的理解并记住它们。

人们期望在一个操作开始前有充足的机会取消它，并且他们期望在执行一个潜在的破坏性操作时得到一次确认他们目的的机会。最后，人们期望可以温和地停止一个正在进行的操作。

### <a name="From Concept to Product"/>From Concept to Product
#### 从概念到产品
#### 定义你的App
一个app的定义声明是一个简洁的、具体的关于app的主要目的和预期受众的声明。

在你的开发早期创建一个定义声明会帮助你将一个想法和一连串的特性转变成一个人们想要拥有的产品。在开发过程中，通过定义声明来决定潜在的特性和行为是否有意义。通过下面的步骤来创建一个稳健的app定义声明。

##### 1、列出所有你觉得用户可能喜欢的特性
进行头脑风暴。在这里，你要试图抓住所有与你的主要产品想法有关的所有任务。不要担心你的清单太长；你之后会缩减它。

想象一下假如你最初的想法是开发一个帮助人们购买食品的app。当你思考这个动作时，你会想出一系列的相关任务——也就是潜在的特性——是用户可能会感兴趣的。比如说：
* 创建清单
* 获取食谱
* 比较价格
* 定位商店
* 注释食谱
* 获取和使用优惠券
* 查看烹饪演示
* 探索不同的菜系
* 寻找原料的代替品

##### 2、确定你的用户是谁
现在你需要思考如何区分你和其他app的用户。在你的主要想法中，对他们最重要的是什么？使用食品购物的例子，你也许要问你的用户是否：

* 通常在家烹饪还是更喜欢熟食
* 是坚定的优惠券使用者还是觉得优惠券不值得付出努力得到
* 享受获取特殊的原料还是很少冒险超出基本原料
* 严格的遵守食谱还是只把食谱当灵感来源
* 频繁地小量购买还是偶尔大量购买
* 想要为不同的目的持有几个进行中的清单还是只想记住少量在回家路上买的东西
* 坚持独特的品牌还是凑合着用最方便的选择
* 倾向于买在每个购物之旅买一套相似的东西还是仅仅买食谱上列出的东西

在思考这些问题之后，想象你决定了三个最能描述你目标受众的特性：喜爱尝试食谱、经常很匆忙并且如果不用耗费太多努力的话乐于节约。

##### 3、通过受众定义来过滤特性清单
如果，在决定一些受众特性之后，你只留下了一小部分的app特性，你就站在了正确的轨道上了：好的iOS app会集中精力于它们帮助用户完成的任务上。

比如说，考虑你在第一步中相处的一长串的可能的特性。即使这些都是有用的特性，但并不是都会被你在第二步中定义的受众所感激。

当你在你目标受众的前提下检查你的特性清单，你认为你的app应该专注于三个主要的特性：创建清单、获得和使用优惠券以及获得食谱。

现在你可以制作你的app定义声明了，具体地总结app会做什么以及为谁做。一个好的为这个食品购物app撰写的定义声明如下所示：

“一个给勤俭并爱烹饪的人们使用的购物清单创建工具。”

##### 4、不要止步于此
在开发过程中使用你的app定义声明来决定特性、控制和术语是否合适。比如说：

`当你考虑添加一个新特性时，`询问你自己这个特性对于app的主要目的和目标受众是否必要。如果不是，那么置之不理；这可能是形成一个不一样的app的基础。比如说，你已经确定了你的用户对冒险的烹饪感兴趣，那么强调盒装混合蛋糕和熟食可能就不会被赞赏。

`当你考虑UI的外观和行为时，`询问你自己你的用户是否喜欢一个简单、精致的风格还是一个更加明显的主题化风格。以人们期待的东西为指南来完成你的app，比如完成一个严肃任务的能力、快速获取答案的能力、钻研综合信息的能力或者娱乐的能力。比如说，虽然你的食品清单app需要易于理解和快速使用，你的受众也许会欣赏一个展示很多漂亮的原料和谷物的图片的主题化UI。

`当你考虑要使用的术语时，`努力和你受众的专业知识所匹配。比如说，即使你的受众也许不是由专业厨师组成的，你也要确信他们会想要看到原料和技巧的恰当说法。

#### 为任务量身定做你的界面
最好的iOS app会处理好定制UI和目标清晰以及易于使用之间的平衡。在你的app中达到这种平衡，确保在设计的早期考虑定制。因为考虑品牌化、原创性和市场能力时经常会影响到定制的决定，集中在定制如何影响用户体验这件事上将会是一件挑战。

从考虑你app的任务开始：用户多久执行他们一次以及在何种情况下执行？

比如说，想象一下一个使用了精心设计的、有艺术感和想象力的布局来展示熟悉的计算元素的计算器。细心绘制的插图和富有想象力的布局并没有影响人们理解如何点击按钮和阅读结果。但是对那些只需要简单地完成工作的人，这种新奇的体验感很快就会消退，而漂亮的定制化UI变成了一种累赘。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/From%20Concept%20to%20Product/1.jpeg)

与此相反，看一下GarageBand。GarageBand本可以在不展现漂亮的、现实的乐器的情况下帮助人们制作音乐，但这样会让app变得不直观且没有乐趣。在GarageBand中，定制化的UI不仅仅告诉人们如何使用app，它还会使主要的功能——即制作音乐——更加易于完成。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/From%20Concept%20to%20Product/2.jpeg)

当你思考定制化会如何加强或者削弱你的app的功能时，记住这些指南。

`定制一定要有理由。`理想上，UI定制化对人们想要完成的任务有利而且会加强他们的体验。你要尽可能地让你的app的功能主导你的定制化决定。

`尽量避免增加用户的认知负担。`用户对标准UI元素的外观和行为很熟悉，所以他们不用停下来思考如何使用它们。当面对一些看起来或执行起来和所有标准元素都不像的元素时，用户也就失去了以往经验的优势。除非你独特的元素使任务执行变得容易，否则用户会不喜欢被强制学习一些不能转移的新方式。

`保持内部统一。`你的定制化UI越多，你的定制元素的外观和行为与你app保持一贯性就越重要。如果用户花时间学习如何使用你创建的不熟悉的控制器，他们会期待能够依靠从你的app中得到的知识。

`始终遵从内容。`因为标准元素太熟悉了，它们不会与内容争夺人们的注意力。当你定制你的UI时，注意确保它不会让人们关心的内容失色。比如说，如果你的app允许用户观看视频，你也许要选择设计定制化的重放控件。无论你使用定制的还是标准的重放控件，是否在用户开始观看时淡出以及在点击时出现都更加重要。

`在你重新设计一个标准控件时要三思。`如果你计划做比定制一个标准控件更多的事，确保你重新设计的控件提供了和标准控件同样多的信息。比如说，如果你创建了一个switch控件而这个控件没有显示相反值的存在，人们就不会意识到这是一个两种状态的控件。

`确保彻底测试定制的UI元素。`在测试过程中，仔细观察用户是否能预期你的元素的功能以及是否能简单地和它们交互。如果，比如说，你创建了一个击中区域小于44*44点的控件，人们要启动它会有困难。或者如果你创建了一个对点击和滑动有不同响应的视图，确保这个视图提供的功能值得用户在和它交互时额外地小心。

#### 原型和迭代
在你投入大量工程资源来实现你的设计之前，创建一个原型供用户测试是一个很好的方法。即使你只能找到很少的同事来测试原型，你也会在他们对你的app的功能和用户体验的新鲜看法中获益。

在你设计的早期你可以使用纸上的原型或者线框来展示主要的视图和控件，并设计视图间的流程图。你会在测试线框时获得一些有用的反馈，但是因为线框太少，也许会误导测试人员。这是因为人们很难想象当线框被真实的内容填充时app的体验会如何改变。

如果你能够提供一个运行在设备上的充实的原型，你将获得更多有价值的反馈。当人们可以在设备上和你的原型交互时，他们会更容易发现哪些地方app的功能与他们预期的不一样，或者哪里的用户体验太过复杂。

最简单的创建可靠的原型的方式是使用基于故事版的Xcode模板来创建一个基础的app，然后填入一些合适的占位内容。（故事版文件包含了你app中的所有UI，也包括不同界面间的跳转。）然后将原型安装到设备上，这样你的测试员就可以有一份尽可能真实的体验。

你不用在你的原型app中提供大量的内容和控件，但你确实需要提供足够的环境来达到真实的体验。以达到典型用户与边缘用户的体验平衡为目标。比如说，如果你的app需要处理一长串物体列表，你就不要在原型中只展示一两个物体的列表。而为了测试用户的交互，只要用户可以点击屏幕的某个区域来跳转到下一个逻辑界面或者执行主任务，就需要给他们提供反馈。

当你的原型基于一个Xcode app模板时，你会免费获得很多功能而且对反馈响应的设计调整也会相当容易。经过简短的回顾，你应该可以在巩固你的设计并付诸实现前测试你的原型的很多次迭代了。查看Xcode Overview开始学习关于Xcode的内容

### <a name="Case Study - From Desktop to iOS"/>Case Study - From Desktop to iOS
#### 案例学习：从桌面到iOS
#### iPad端的Keynote
桌面端的Keynote是一款强大的、灵活的创造世界级幻灯片的app。人们因Keynote很好地结合易于使用与无数细节打造的细粒度控制而喜爱它，比如动画和文本属性。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/1.jpeg)

iPad端的Keynote把握了桌面端Keynote的精华，并通过创造如下的用户体验使其在iPad上宾至如归：
* 专注于用户的内容
* 降低复杂性而不减少功能
* 提供快捷方式
* 改编桌面端体验上熟悉的内容
* 通过生动的动画提供反馈和交流

由于通过使用iPad原生的模式来提供期待的功能，Keynonte用户能够很快明白如何在iPad上使用app。新用户也能很容易地学会如何在iPad上使用Keynote，因为他们可以通过简单、自然的方式直接操控他们的内容。

Keynote从桌面端到iPad端的转变是基于无数从细微到深入的修改和重设计的。这里是一些最明显的适应性改编：

`一个精简的工具栏。`工具栏上只有少量的元素，但它们使用户能够始终获取他们创造内容所需要的功能和工具。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/2.jpeg)

`一个简化的、主次排列的检查器来响应用户的关注。`iPad端的Keynote检查器会自动包含人们在修改所选中的物体的时候需要的工具和属性。基本上人们可以在检查器的第一页获取他们需要的所有内容。如果他们需要修改一些较少改变的属性，他们可以继续到别的检查器界面获取。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/3.jpeg)

`很多的预置风格集合。`人们可以通过预置的风格来简单地改变物体的外观和感觉，例如图标和表格。除了颜色方案，每种集合都包括了对应风格的属性，比如表头和坐标轴标识，它们被设计成与所有主题相协调。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/4.jpeg)

`直接操控内容，并且配有合乎意义的动画。`在iPad端的Keynote上，用户拖动幻灯片使其到新的位置，扭转物体使其旋转，以及点击图片来选中它。直接操控的印象为iPad端的Keynote执行的响应动画所加强。比如说，当用户移动幻灯片时，它会轻轻地震动一下，当他们将幻灯片放置到一个新的位置时，周围的幻灯片会像波纹一下向外扩展来给它提供空间。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/5.jpeg)

`直接操控内容，并且配有合乎意义的动画。`在iPad端的Keynote上，用户拖动幻灯片使其到新的位置，扭转物体使其旋转，以及点击图片来选中它。直接操控的印象为iPad端的Keynote执行的响应动画所加强。比如说，当用户移动幻灯片时，它会轻轻地震动一下，当他们将幻灯片放置到一个新的位置时，周围的幻灯片会像波纹一下向外扩展来给它提供空间。

#### iPhone端的邮件
在OS X系统中邮件是最高可见的、好用的以及受赞誉的app之一。它也是一个非常强大的创建、接收、排序、存储邮件；追踪行动项目和活动；创建备注和请帖的程序。桌面端的邮件使用了很多的视窗来呈现这些强大的功能。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/5.jpeg)

iPhone端的邮件专注于桌面端邮件的核心功能，帮助人们接收、创建、发送和管理他们的邮件。iPhone端的邮件使用了如下为移动端体验定制的UI来提供这些浓缩的功能：
* 流线型的外观使人们的内容前置居中
* 为不同的任务设计不同的视图
* 可以轻松缩放的直觉性的信息结构
* 在需要的时候提供强大的编辑和管理工具
* 使用精妙而有表现力的动画来与动作交互并提供反馈

要认识到iPhone端的邮件并不是一个比桌面端邮件更好的app，而是一个重新为移动端用户设计的邮件app。通过集中精力与桌面端的部分特性并使用愈加迷人的UI展示它们，当他们使用移动端的时候，iPhone端的邮件给予了人们邮件的核心体验。

为了使邮件的体验符合移动端的环境，iPhone端的邮件使用了很多关键的方式创新UI。

`清晰的、高关注度的屏幕。`每个屏幕都展示了邮件体验的一部分：账户列表、邮箱列表、邮件列表、邮件视图以及新建邮件视图。在一个屏幕上，用户可以滑动查看所有内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/Design%20Strategies/Case%20Study%20-%20From%20Desktop%20to%20iOS/6.jpeg)

`简单、可预测的导航。`点击每一个屏幕，人们会从一般界面（账户列表）进入到特殊界面（邮件视图）。每个屏幕都展示了一个标题来告诉人们他们在哪，以及一个返回按钮使人们可以简单地回到之前的步骤。

`简单、可点击的控件会在需要的时候显示。`因为创建一封新邮件以及检查新邮件是人们也许会在任何环境下都想要的基本功能，iPhone端的邮件使它们在很多屏幕上均可获取。当人们查看一封邮件时，诸如回复、移动和删除功能都是可获取的，因为他门正在操作一封邮件。

`不同的任务有不同类型的反馈。`当人们删除一封邮件时，它会有进入删除按钮的动画。当人们发送一封邮件时，他们可以看到这个过程；当发送结束时，他们可以听到一声有特色的声音。通过查看邮件列表工具栏的精细文本时，人们可以瞥一眼就知道他们的邮箱上一次更新是什么时候。

#### iOS端的Web内容
iOS端的Safari提供了iOS设备中杰出的移动Web浏览体验。人们欣赏其简明的文字、锐利的图片以及通过旋转设备或点击屏幕来调整他们的界面的能力。

标准的网页能在iOS设备上良好地显示。特别是那些识别设备并且不使用插入式的网页可以在iPhone和iPad上都显示得很棒，即使需要调整也只是一点点。

除此之外，最成功的网页有以下特性：
* 如果网页的宽度需要匹配设备的宽度的话，为设备设置合适的窗口
* 不要使用CSS固定定位，这样当用户调整视图的时候内容就不会移出屏幕
* 使用不依赖于点交互的基于触摸的UI

有时候，其他的修改也会合适。比如说，网页程序总是设置适当的窗口宽度并隐藏iOS端Safari的UI。查看Safari Web Content Guide中的Configuting the Viewport和Configuring Web Applications学习如何做这些修改。

网页也可以使用其他方式来使桌面Web体验适应iOS端的Safari：

`协调iOS端Safari中的键盘。`当键盘和格式助手可见的时候，iPhone中的Safari会在URL文本内容以下、键盘和格式助手以上的区域显示你的网页。

`协调iOS端Safari中的弹出菜单控件。`在桌面端的Safari中，包含大量内容的弹出菜单会像在OS X的app中一样显示；也就是说，菜单会打开来显示所有的内容，如果必须的话甚至会超出窗口的边界。而对于iOS端的Safari，弹出菜单是使用原生的元素显示的，因而提供了一个更好的体验。比如说，在iPhone上，弹出菜单通过一个选取器（一个用户可选的内容组成的列表）来显示。（查看Picker学习更多关于选取器控件的内容）。

## <a name="iOS Technologies"/>iOS Technologies
### <a name="3D Touch"/>3D Touch
#### 3D Touch
3D Touch让iOS 9的用户多了一个交互的维度。在支持的设备上，人们可以通过按压主屏幕上的app图标来快速地选择其特有的操作。在app内，人们可以使用多种压力来获取一个内容的预览、在另一个视图打开内容以及获取相关的操作。（查看Adopting 3D Touch on iPhone来学习更多关于在你的代码中支持3D Touch的内容。）

#### Peek 和 Pop
Peek让用户可以在不离开当前环境的情况下预览一个内容以及执行相关的操作。元素通过在轻按时显示一个小的矩形视图（有时称为hint）来表明其支持peek。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/3D%20Touch/1.jpeg)

peek：
* 在用户按一个支持peek的元素时显示，在用户手指离开时消失
* 当用户在peek视图上稍微按深一点时，打开一个元素的详情视图——称为pop
* 当用户在peek视图上向上滑时，会提供关于元素的快捷操作

当用户轻按屏幕时，支持peek的元素会通过展示一个你提供的矩形视图来暗示有更多的交互可获取。这个视图要够大，这样用户的手指才不会挡住内容，还要够详细，这样用户才能决定是否要按深一点来查看peek视图。

`重要`
使用peek和pop要贯穿整个app，这点很重要。如果你在一些地方提供peek和pop，而在另一些地方不提供，用户会觉得你的app或者他的设备出了问题。

`使用peek来提供元素的一个生动的、内容丰富的预览。`peek最好能给用户关于元素足够的信息来补充他们当前的任务。比如说，用户可以使用peek来预览信息中的一个URL对应的网页，这样他们就可以决定他们是否要在Safari中打开网页或者分享链接给他们的朋友。在一个列表视图中，peek给用户展示某一行的详细视图。

`为每个peek提供一个pop。`即使peek应该给用户大部分他们需要的信息，你也应该始终让用户在决定离开当前任务并关注元素内容的时候可以跳转到pop。pop应该和用户点击元素时获取到的视图一样。

`不要为同一个元素同时提供peek和编辑菜单。`当同一个元素的两种特性都提供时会变得迷惑。（查看Edit Menu来学习更多关于编辑菜单的内容。）

`在peek内，不要显示看起来像按钮的元素。`如果用户松开他们的手指去点击那个看起来像按钮的元素，peek就会消失。

`如果合适的话，提供peek快捷操作。`在peek内，用户可以通过上滑显示与元素相关的操作。比如说，邮件的peek快捷操作包括回复所有、跟随和移动邮件。不是所有的peek都需要快捷操作，但如果你已经为元素提供了自定义的长按操作，为元素使用peek提供同样的操作代替长按是一个好的做法。（注意网页peek的快捷操作是自动提供的。）

`不要将peek作为获取元素特有操作的唯一方式。`不是所有设备都支持peek和pop，而且有些用户可能会选择关闭3D Touch功能，所以寻找其他方式来使peek的功能在你的app中可获取是必要的。当你的app运行在旧设备中时，在用户长按元素时让他们获取到与peek快捷操作相同的view是有意义的。

#### 主屏幕快捷操作
主屏幕快捷操作给了用户一种方便的在主屏幕执行有用的、app特有的操作的方式。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/3D%20Touch/2.jpeg)

主屏幕快速操作：
* 当用户使用比长按app图标深一点点的方式点击主屏幕上的图标时出现
* 展示一个短标题、一个图标以及可选的你提供的子标题
* 不支持其他自定义内容
* 当你的app更新时能展示新的信息

`使用主屏幕快捷操作提供引人注目的、高价值的任务。`比如说，地图可以让用户在不首次打开地图app的情况下搜索他们位置附近的东西或者获取家的方向。每一个app都应该至少提供一个主屏幕快捷操作的有用的任务；你可以提供总共四个快捷操作。

`不要使用主屏幕快捷操作来快速导航你的app。`如果用户访问你app的重要内容很难或者很花时间，首先修复你app的导航，这样所有的用户都可以受益。然后专注于提供那些深入链接你app或者完成有用的、有创意性任务的主屏幕快捷操作。

`不要以用户难以预期的方式改变主屏幕快捷操作。`最好基于用户理解的事件或环境改变来更新快捷操作。比如说，基于用户在你app中当前的位置或者最近的操作、事件或者用户设置的改变来更新元素会比较有意义。

`不要使用主屏幕快捷操作来作为通知用户的方式。`iOS的用户期待通过别的方式来获取app的通知（查看Notifications来学习这些方式）。

`为每个主屏幕快捷操作提供一个简洁的标题（以及可选的子标题）和一个模板图标。`标题应该立即显示操作的结果；比如说，“家的方向”，“创建新联系人”和“新信息”。你也可以提供可选的子标题来给用户更多的内容。比如说，邮件在VIP主屏幕快捷操作中使用了子标题来告诉用户他们是否有未读邮件。不要在标题和子标题中包含你的app名称或任何外部信息，并且确保在写文本的时候考虑位置。

保持标题尽可能的短很重要，这可以避免被截断并且能帮助用户快速理解操作。如果你提供子标题，系统会截断太长的标题来适应一行；如果你不包含子标题，系统会将长标题截断显示到第二行去。

你可以从很多系统提供的模板化图标中选择或者你也可以自己创造一个自定义的模板化图标。从[https://developer.apple.com/design/downloads/Quick-Action-Guides.zip](https://developer.apple.com/design/downloads/Quick-Action-Guides.zip)下载主屏幕快捷操作图标模板来获取关于图标尺寸、内边距以及位置的指南。查看Template Icons来学习更多关于设计一个模板化图标的内容。

系统会自动在快捷操作列表的左边或右边显示图标，这取决于你的app图标在用户主屏幕上的位置。（无论图标在列表的什么位置，文本都是左对齐且从左读到右的。）这里是一些主屏幕快捷操作的例子，展示了他们的不同显示形式。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/3D%20Touch/3.jpeg)

### <a name="Live Photos"/>Live Photos
Live Photos可以让用户捕获并通过一个简短的、充满动感的体验重现一段他们最喜爱的记忆。从iOS 9开始，相机app会捕获额外的内容——包括声音以及照片前后额外的帧——来将生活添加到传统的静止图片中。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Live%20Photos/1.jpeg)

在iOS 9.1以及之后的系统运行的app中，你可以让用户在你的app内享受并分享Live Photos。这里的指南可以帮助你给予用户一个好的体验。

`在不支持Live Photos的环境中将Live Photo用传统图片显示。`不要在支持Live Photo的环境下使用自定义实现的类似Live Photo提供的体验。

`不要分开显示Live Photo的额外的帧和声音。`在整个app中使用相同的视觉效果和交互模式给用户一个统一的Live Photo体验很重要。拆开Live Photo来显示分开的部分会给用户一个很差的体验。

`确保用户能够区分Live Photo和传统的静止图片。`尤其是当用户可以分享图片时帮助用户区分这一点很重要。最好的告诉用户他们正在看一个Live Photo的方式是显示一点运动来提供一个hint体验。如果是在不能用hint的地方，你可以显示系统提供的Live Photo 的标记。Live Photo从不显示看起来像一个视频的回放按钮。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Live%20Photos/2.jpeg)

`注意`
当用户在照片app中使用全屏浏览照片时不支持视觉运动效果。

`对Live Photo的所有帧使用用户调整的内容。`如果你的app允许用户对照片添加效果或调整，确保更新整个Live Photo。如果你不支持调整用户希望分享的整个Live Photo，让他们知道他们只能将其作为一个传统图片分享。

`在用户决定分享之前让他们预览Live Photo的所有内容。`如果你的app包含帮助用户选择照片去分享的UI，引入一种方式让他们可以将Live Photo作为传统照片分享。

`如果你使用了系统提供的标记，在每张Live Photo上都将其放在同样的位置。`一般将标记放在照片的一角是比较好看的，这样它就不会干扰到用户查看照片。确保在你整个app中都使用标记这样用户就可以依赖它来识别Live Photo。iOS提供了两种风格的标记图片：
* 覆盖。覆盖风格包含一个阴影使其在照片内容上方看起来不错。
* 固色。固色风格（不包含阴影）可以被用来创建你可以调色的模板图片。

  iOS也为固色风格提供了很多标记，包括图片上的中划线来表示这个Live Photo现在被当成传统照片对待。
 
`当用户下载Live Photo时给他们好的体验。`尤其是用户需要知道他们正在下载的是一张Live Photo以及他们何时可以播放它。如果你显示一个加载显示器来说明一张Live Photo还不能播放，确保使用与你app中其他下载体验一致的加载显示器。

### <a name="Wallet"/>Wallet
#### 钱包
Wallet（钱包）帮助人们查看和管理Pass（凭证），这是一种类似于登机牌、优惠券、会员卡、奖励卡和各种票的物理凭证的数字替代。Wallet也允许人们添加信用卡、借记卡和储值卡来和Apple Pay一起使用。在你的app中，你可以创建一个Pass，将其分配给用户，然后当内容更改时更新它。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Wallet/1.jpeg)

PassKit 框架使自定义内容来接收Pass以及当用户的Pass库中有它的时候使用Pass变得容易。（查看Wallet Developer Guide来学习关于Wallet的主要技术以及如何在你的app中使用PassKit API。）下面这些指南可以帮助你创建一个人们乐于放在Wallet中并享受使用它的Pass。

`设计在所有设备上都好看的Pass。`当你选择一种Pass风格——例如登机牌、优惠券、票、奖励卡或者通用的pass——你会获得一个独特的布局和很多可以编辑的区域（查看Pass Style Sets the Overall Visual Appearance获取不同pass风格的细节）。系统会在每个设备上恰当地显示你的pass，所以正确地使用pass的区域很重要。比如说在Apple Watch上，strip和略缩图是不显示的，所以你不会想把必要的信息放在这些区域中。查看Designing Passes for Apple Watch学习更多关于Apple Watch上pass布局的内容。

`使用合适的pass区域来显示文本。`使用区域让旁观用户可以获取你pass中的所有信息，并给你的pass一个一致的外观。还应该避免在图像上放置文字和使用自定义的字体，因为不是所有的设备都会显示所有的图片，并且自定义的字体会让用户读起来很困难。

`不要使用依托于设备的语言。`你无法预期你的用户会在什么设备上查看你的pass，所以你不会想使用在一些特殊的设备上没有意义的语言。比如说，告诉用户去“滑动界面”的文字内容在Apple Watch上没有意义。

`尽可能地避免简单地复制已经存在的物理凭证。`Wallet有着确定的设计美学，而和这种美学结合的pass看起来是最好的。不要复制物理pass的外观，使用这个机会去设计一个遵循Wallet形式和功能的清晰的、简洁的pass。

`你放在pass前面板的信息要有讲究。`人们期待可以看一眼pass就很快地获取他们需要的信息，所以pass的前面版应该整洁且易于阅读。如果有其他的信息你觉得用户也许会需要，将他放在pass的背面板比挤在前面板要好。注意Apple Watch上的pass不包含背面板。

`避免使用平淡的白色背景。`pass会在背景是一个鲜明的、立体的颜色或者是使用强烈的生动的颜色的图片时看起来最好。当你设计背景时，永远要确保它不会干扰到内容的可读性。

`为你的公司名使用logo文本区域。`logo文本区域的文本会在所有的pass上使用一致的字体渲染。为了避免和Wallet里的其他pass冲突，推荐你将文本放在logo文本区域而不是使用自定义的字体。

`使用一个白色的公司logo。`logo图会放在pass的左上角，靠近你的公司名。提供一个单纯白色版本的不包含文字的logo会是最好的。如果你想要装饰logo来和渲染的logo文本相匹配，添加一个1像素Y位移、1像素模糊、35%透明度的黑色阴影。

`可能的话使用一个矩形的条形码。`由于pass的布局，一个矩形的条形码——例如PDF417——会比方形的二维码看起来好。如下右图所示，方形的二维码会在两边形成空白区域而且会在垂直方向上使上面和下面的区域变得拥挤。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Wallet/2.jpeg)

`性能最好的图片。`由于用户经常通过邮件或Safari接收pass，使下载尽可能的快很重要。为了提升用户体验，使用能达成想要的视觉外观的最小的图片文件。

`当合适的时候更新pass来加强它的实用性。`即使pass是用来代替基本不会更改的物理凭证的，你的数字pass也可以通过反映现实世界的事件来提供更好的体验。比如说，你可以在飞机延误的时候更新航空登机牌，这样用户就总是能在他们查看pass的时候获取当前的信息。

### <a name="Apple Pay"/>Apple Pay
#### Apple Pay
Aplle Pay是iOS设备上一种易用的、安全的、私有的支付方式。当使用app购买物理商品和服务时，人们可以使用Apple Pay来快速、安全地提供支付对象、运送方式和支付信息。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Apple%20Pay/1.jpeg)

通过使用Apple Pay，人们可以不用创建账户和输入信息来进行支付。Apple Pay大大地加速了支付的过程，帮助去除了前期的注册流程，并给用户提供了一个浏览你产品和轻松购买的更好的体验。查看Apple Pay Programming Guide获取更多信息。

Apple Pay的UI是清晰的、精简的、不引人注目的。在不同的环境下有三种展现形式：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Apple%20Pay/2.jpeg)

`按钮。`Apple Pay的按钮告诉用户他们可以在当前环境进行购买，例如产品页面。当用户点击Apple Pay按钮时，立即显示一个支付表格（下面会描述）并帮助他们开始付款过程。Apple Pay的创建按钮让用户可以创建Apple Pay。你可以使用PKPaymentButton API来获取这些按钮（查看PKPaymentButton Class Reference来学习更多）。查看Apple Pay Identity Guidelines来获取更多关于使用Apple Pay按钮的信息。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Apple%20Pay/3.jpeg)

`Apple Pay标记。`用户期望当他们需要选择一个支付选项和在授权一次支付前完成额外的信息时看到Apple Pay标记。Apple Pay标记应该只在其他支付选项也以相同或类似的格式显示的时候出现。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Apple%20Pay/4.jpeg)

`支付表格。`在一个用户提交一个订单和相关的支付前，Apple Pay要显示一个支付表格显示他们支付相关的支付对象（CONTACT）、运送方式（SHIPPING）和支付信息。即使人们可以在支付表格中进行一些修改——比如选择一个不同的运送方式——他们也不需要输入额外的信息。当用户查看支付表格时，他们应该能够立即完成交易并授权支付。

`始终对能够使用Apple Pay的人显示Apple Pay UI。`当用户在一个支持的设备上并且激活了你提供的卡的时候，这表示他们想要在你的app中使用Apple Pay。将Apple Pay设为默认的支付选项来满足用户的期待。

`如果一个用户不能使用Apple Pay，不要显示任何Apple Pay的UI。`如果用户正在使用一个不支持Apple Pay的设备，将其作为一个支付选项会引起迷惑。然而，如果用户正在使用一个支持Apple Pay的设备，但没有创建信用卡或借记卡，你可以显示创建Apple Pay按钮。

`在用户点击Apple Pay按钮之后立即显示支付表格。`强制你的用户在决定开始使用Apple Pay支付之后进行额外的步骤会增加这个过程的阻力并阻挠你的用户。不要在用户点击Apple Pay按钮之后显示额外的警示框和模态视图。如果用户能够提供类似折扣代码和促销代码的东西，找到方法来在他们点击Apple Pay按钮之前获取这个信息。

`使用与其他可见的支付按钮同样的或者更大的按钮来显示Apple Pay按钮。`显著地显示Apple Pay按钮来帮助用户更容易找到它。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Apple%20Pay/5.jpeg)

`使用Handoff来帮助用户完成他们在Apple Watch上创建的支付。`Apple Watch的穿戴者可以在app store进行购买，但他们不能再你的Apple Watch app中完成一个购买。当用户在你的Apple Watch app中创建一个购买时，显示一个信息告诉他们到他们的iPhone上完成支付。最好的体验是，使用Handoff来与你的iOS app建立深度联系并且立即显示一个预填充合适的信息的支付表格。

查看Apple Pay Identity Guidelines获取更多关于如何使用Apple Pay按钮和标记的指南。

#### 自定义支付表格
你可以自定义Apple Pay支付表格的样式，这取决于你完成交易需要知道的信息和你需要传达给用户的关于购买的信息。

`只在支付表格上显示完成交易必须的信息。`如果Apple Pay支付表格显示了无关的信息，用户也许会感到困惑或担心。比如说，当电子化地产品将被交货或者实现的时候，请求一个联系人的邮箱地址就有意义，但运送方式就没意义。在这个例子中请求一个运送方式会给用户一种有东西要被意外地送到他家或者公司的印象，或者让他们担心他们的信息被不必要地使用了。

`在支付表格内让用户选择一种运送方式或收货方式。`用户可以在Apple Pay支付表格中从你指定的任意种方式中选择一个收货方式。使用一个文本、一个花费信息和一个可选的第二行来提供预期的收货日期来指定一种运送方式。或者，你可以将表头从“Shipping”改成“Pickup”来让用户指定一个物体的位置，比如一个快递服务的收货快递员。

`为重复支付和要添加到购买总费用的费用使用行元素。`一个行元素由一个文本和一个花费信息组成。使用行元素来：
* 使用像“每月捐献$19.99”的行元素表明一个用户在授权一个重复支付
* 提醒用户额外的花费，比如“礼物包装$5.00”或“税$4.53”
* 显示可以减少花费的赠券或者折扣，例如“周五折扣 -$2.00”
* 显示一个待定金额，例如快递服务的“时间&距离...”

不要使用行元素来显示组成购买的产品的列表。

`尽可能地创建能在一行显示的行元素文本。`行元素文本应该明确且易于被用户理解。创建冗长的文本会让你的用户很难看一眼就理解行元素。

`于同一行内在“PAY”后面提供一个统一的商户名。`确保使用同样的商户名，用户会在检查他们的信用卡和银行账单时查看相关的花费。这很重要，因为这会帮助用户确保他们的支付到了他们想要支付的地方。如果你的app是扮演一个中间人的角色，并不是支付最终的店主，通过说明“PAY ‘最终商户名’（通过 ‘你的app名’）”清晰地告诉用户这一点。

`如果总花费是未知的，在授权支付的时候传达也许会有额外的花费这个信息。`比如说，对于一个基于距离和时间的行车，从发出这个购买到授权支付，价格有可能会改变。或者消费者也许会在产品发送后增加一个小费。在这种情况下，在支付表格中提供一个非常清晰的说明是必要的。如果你使用了一个行元素来更新最终花费，金额就会自动显示为“金额待定”。同样地，如果你预授权一个有明确金额的支付，确保支付表格正确地反映了这个信息。

#### 精简支付过程
人们喜欢快速、简单地使用Apple Pay来进行他们的购买。越少的支付步骤，用户需要手动输入的信息越少，越好。始终使用Apple Pay中最新的信息。假设用户保持他们的Apple

`Pay信息完善且最新，并且不依赖于任何早期收集的信息。`即使你以前收集了用户的联系人、运送方式或者支付信息，在支付时也要提取Apple Pay的最新信息。不要让用户在支付时输入任何你可以从Apple Pay取到的信息。

`使用Apple Pay来加速购买。`要完成单个商品的购买，让用户点击产品界面的Apple Pay按钮来显示支付表格并完成一次立即的支付。用户喜欢不用通过额外的步骤去将商品添加到购物车就能在你的app中购买单个的商品的便利性。对于购物车中的多件商品要以同样的方式送往同样的地址这种情况，支持一个快速的支付流程让用户在准备好支付时尽快地显示支付表格。

`在显示支付表格前收集返现或推广代码。`因为没有方式去在Apple Pay支付表格中输入代码，确保在显示表格前收集代码。

`如果人们可以在一个购物车内配送独立的商品去不同的地方或者以不同的速度配送。`在显示支付表格前获取这个信息。在这个少见的情况中，你需要在显示支付表格前获取配送信息，因为没有方式可以在支付表格内指明多种配送方式或地址。在一般情况下，确保在支付表格内收集配送方式和地址信息。

`显示一个清单确认界面或者谢谢界面。`为了提供一种连贯的用户体验，在支付完成后，使用一个订单确认界面来显示关于产品何时会派送以及用户如何查看他们订单状态的详细信息。

`合适的话，在你的确认界面标注Apple Pay。`虽然在你的确认屏幕上提及Apple Pay不是必要的，如果你选择去提及，使用这些形式：
* “Visa····1234(Apple Pay)”
* “使用Apple Pay支付”

### <a name="Research Apps"/>Research Apps
#### 研究型App
研究型App使iOS用户可以利用他们iOS设备的便利性参与到研究工作中去。Apple的开源ResearchKit工程中初步设计的界面和可获取的跳转使得创建一个漂亮的研究型app变得很容易，这个app可以根据你的研究来定制并且会让人们乐于使用。查看researchkit.org学习如何使用[ResearchKit](http://researchkit.org)来为你的研究开发一个研究型的app。

`重点`
这些指南仅供参考，不构成法律意见。你应该联系律师获得关于研究型app开发方面和其他适用的法律方面的建议。

一般来说，一个研究型app组会自定义ResearchKit界面和app独特的界面来契合三个基本的体验：
* 信息载入
* 研究相关的调查
* 管理条目

遵循这三个体验组成的指南，你就能设计一个帮助参与者感到舒适并保持使用的研究型app。

#### 信息载入
信息载入体验由一系列的部分组成，包括向潜在的参与者介绍研究和让你获取他们的同意。参与者一般在完成这些信息载入部分之后不会再次访问。信息载入体验包含这些部分：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/1.jpeg)

你应该在信息载入体验部分提出这些内容——即介绍、资格、授权以及（如果合适的话）使用信息的许可。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/2.jpeg)

`创建一个介绍来通知并提供一个活动的号召。`介绍版块应该帮助人们了解更多关于你研究的信息并告诉他们如何成为一个参与者。最好还为已经是参与者的人提供一个登录的快速方式并继续完成在进展中的调查。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/3.jpeg)

`尽快地确定资格。`在介绍版块之后、授权版块之前显示一个资格版块（如果参与者不符合调查的资格那就不需要看到授权版块）。确保只显示对你的调查必要的资格需求。使用简单、直观的语言来描述需求并让人们能简单地输入信息。

`在你获取参与者的授权之前确保他们了解你的调查。`ResearchKit可以帮你使得授权过程简明而友好，且允许你在授权中包含法律许可或者机构审查委员会或伦理审查委员会设置的许可。（如果你的app包含人体研究，你必须确保你的app遵守相应的App Store指南，包括同意许可。）一般来说，授权版块：
* 解释调查是怎样进行的
* 确保参与者理解调查以及他们的职责
* 获取参与者的授权

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/4.jpeg)

`将长篇的授权文章拆分成易于消化的子章节。`每个子章节可以涵盖调查的一个方面，例如数据采集、数据使用、潜在的好处、可能的风险、付出的时间、如何撤回等等。对每一个章节，使用简单、直观的语言提供高度的概括。如果必要的话，提供一个子章节的详细说明让参与者点击一个了解更多按钮就可以阅读。参与者应该在他们同意参与之前能查看到整个的授权内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/5.jpeg)

`如果有意义的话，提供一个小测验来测试参与者对调查的理解。`如果你亲自去获取参与者的授权你也可能选择去问同样的问题。

`获取参与者的授权，并且如果合适的话，获取一些联系信息。`同意参与调查之后，参与者会收到一个确认对话框，按照下方屏幕的方式让他们提供他们的签名和联系信息。大部分的研究型app会给参与者发一封PDF形式的知情同意书让他们保留。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/6.jpeg)

如果你需要使用参与者的设备或数据，要获得许可。清晰地解释为什么你的研究型app需要使用定位、健康app或其他数据，并且确保不要询问使用对你的调查不关键的数据。如果你的app需要的话，发送通知到参与者的设备也要获得许可。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/7.jpeg)

#### 调查特有的调查问卷
为了获取参与者的输入，你的调查必须使用调查问卷、活动性任务，或者两者兼而有之。依赖于你调查的结构，参与者会和每个版块交互一次或多次。

`创建能使参与者保持专注和使用的调查。`ResearchKit让显示需要不同类型答案的调查问题变得简单，比如对或错、多选、日期和时间、滑动范围以及开放性地输入文本作为结束。当你使用ResearchKit界面创建调查问卷时，遵循下面这些指南来提供一个好的用户体验：
* 告诉参与者有多少问题以及完成调查需要多少时间
* 每个问题使用一个界面
* 在调查过程中向参与者展示他们的进度
* 使调查过程尽可能地短。多个短调查比一个长调查要好
* 对于需要额外说明的问题，为问题使用标准字体，为说明文字使用稍微小一点的字体
* 当调查完成时告知参与者

ResearchKit提供了很多自定义的界面，你可以在你的调查中使用它们。这里是一些调查界面的例子。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/8.jpeg)

`使活动性的任务易于理解。`一个活动性的任务要求参与者保持一个活动，比如对着麦克风讲话、将他们的手指按在屏幕上或者进行一个记忆测试。遵循这些指南来鼓励参与者执行一项活动性任务或者使他们成功的机会最高：
* 使用每个人都能理解的清晰、简单的语言来描述如何执行任务
* 说明任务是否必须在一个特殊的时间或者情况下执行
* 确保当任务完成时告知参与者

这里是两种ResearchKit支持的活动性任务例子。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/9.jpeg)

#### 管理条目
ResearchKit提供了一个资料界面给用户在你的研究型app中管理他们的个人信息。此外，创建一个界面来激励用户并让他们可以追踪他们在调查中的进度是一个好主意。大部分情况下，参与者应该能够在任何时候进入这两个界面。

`使用一个资料界面来帮助参与者管理个人信息和关于你调查的内容。`资料界面可以让参与者编辑在调查过程中能够改变的资料——例如重量或者睡眠习惯——并且提醒他们即将到来的活动。你也可以使用资料界面给参与者一个简单的方式去离开调查并查看授权文档和app的隐私政策。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/10.jpeg)

`使用一个仪表板来激励参与者和显示进度。`一个仪表板界面能够鼓励参与者继续调查。如果对你的调查合适的话，你可以使用仪表板给参与者一个丰富的反馈，比如每日进度、每周测验、特殊活动的结果、甚至将参与者的结果和调查的其他结果的总和进行对比。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Research%20Apps/11.jpeg)

### <a name="App Extensions"/>App Extensions
#### App扩展
App扩展增加了你app的延伸，让用户在使用其他app时可以关注你app的部分功能。比如说，挡在Safari中查看网页时，人们可以使用你的分享扩展来将一个图片或者文章贴到你的社交网站。或者当使用照片时，人们也许会使用你的图片编辑扩展来给图片加滤镜。（在这种情况下，Safari和照片称为host app，因为他们给了用户扩展的链接。）

你提交应用到App Store时交付了一个app扩展功能齐全的iOS app（一个包含扩展的app称为包容性app——containing app）。在你的包容性app中添加扩展以后，人们可以在使用其他app时通过扩展执行快速任务。比如说，当在邮件中阅读一个商品时，人们也许会使用你的动作扩展来添加一个商品到购物清单中去而不用离开邮件。

表22-1列出来很多你可以创建的iOS app扩展

表22-1 app扩展类型  

app扩展类型 | 人们使用扩展来 
----------  | ------------- 
桌面日历    | 在通知中心的日历视图中获取快速更新或者执行快速任务 
分享        | 将网页或者内容分享给他人 
动作        | 在其他app环境下操作或者查看内容
图片编辑    | 通过图片aoo编辑图片或者视频
文档提供者  | 连接并管理一个文件仓库
自定义键盘  | 使用自定义的键盘代替iOS系统键盘

下面的指南对所有类型的app扩展都适用；对于每种app扩展类型各自的指南，查看下面的章节。（查看App Extension Programming Guide学习如何开发、调试和发布一个扩展。）

`完成简单的任务。`app扩展不是你app的迷你版本。相反，扩展执行用户大目标下的一个小任务。比如说，一个动作扩展也许会给用户一个不同的方式去查看他们当前的内容。

`保持用户交互有限且直接。`最好的app扩展让用户只通过很少的点击来执行任务，这样他们就可以尽可能快地回到之前的环境。比如说，一个分享扩展也许会让人们通过一次简单的点击就发布一张图片。

`将你包容性app的名字包含到每一个它提供的扩展的名字中去。`即使包容性app中的多个扩展都应该有唯一的名字，你也希望确保用户理解你的扩展和你的app的关系。人们会在很多不同的环境遇到扩展，并且他们不会信任他们不能识别的而扩展。

`在绝大多数情况下，使用包容性app的图标。`使用一个熟悉的图片是另一种扩展获取用户信任的方式。注意对于动作扩展，要创建一个单色版的app图标（查看[Share and Action Extensions](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/AppExtensions.html#//apple_ref/doc/uid/TP40006556-CH67-SW3)获取细节）。

`重点`  
当你设计图标和图片时，不要复制iOS的图片或图片，也不要创建苹果产品和设计相关的图片。

`不要在扩展的顶层显示modal视图。`很多扩展默认以modal视图来显示，最好避免绘制modal视图。即使有些例子中用户会在扩展的顶层看到一个警告框视图，也要避免设计一个需要modal视图的扩展工作流。

#### “今天”小部件
人们在通知中心的“今天”区域查看“今天”小部件。因为人们会设置今天区域，所以这里显示的是他们最关心的信息，以在用户最重要的条目中占领一席之地为目标设计你的小部件。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/1.jpeg)

`设计看起来与通知中心相协调的外观。`当你使用通知中心提供的默认的边界和背景样式时，你的今天小部件就会给用户一种一致的体验。为了获得最好的结果，集中精力于绘制你的内容而不是背景或别的什么。尤其避免绘制一个立体的背景。

`NOTE`  
iOS会自动在你自定义的小部件上方显示你app的图标和标题（图标会显示在前缘空白）。

`使内容与小部件标题对齐。`当你的小部件与你的标题对齐时，人们可以简单地浏览他们想要的小部件的今天视图。遵循今天视图的边界，并且约束你显示在小部件内容区域的内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/2.jpeg)

`一般来说，使用白色的系统字体来显示文字。`白色文字在通知中心的默认背景下显示的很好。对于次级文本，使用系统提供的活力外观（查看[notificationCenterVibrancyEffect](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIVibrancyEffect/index.html#//apple_ref/occ/clm/UIVibrancyEffect/notificationCenterVibrancyEffect)学习关于这种外观的更多内容）。

`提供通知中心的体验。`人们访问通知中心来获取简单的更新或者执行一个非常简单的任务，所以你的今天小部件最好显示正确数量的信息以及有限的交互，尤其是：
* 不要让用户滚动或者垂直转移视图来查看你的今天小部件的所有信息。小部件可以垂直扩展来显示更多信息，但小部件的高度超过通知中心的高度并不是一个好的体验，因为这使得查看其它今天小部件被滚动干扰了。
* 不要实现水平的点击或者拖拽，因为这和通知中心区域的导航冲突了。
* 尽可能地让用户通过一次点击就可以执行任务或者打开你的app（注意键盘在今天小部件是不能获取的）。
* 优化性能使用户可以立即获取有用的信息。缓存信息到本地是个好主意，这样你就可以在你更新的时候显示最近的信息。人们期待在今天视图中花费非常少的时间，而且iOS会终止那些不经常使用内存的今天小部件。

如果合适的话，让人们点击你的今天小部件去打开你的app。因为你的今天小部件提供了一个紧致的集中体验，引导人们进入你的app获取更多信息和功能会很好。提供一个“打开App”的按钮不是个好主意，所以一个解决方法是让你的整个今天小部件可点击。或者你也可以让用户点击一个小部件内合适的UI部件来打开你的app并进入到关于那个部件的视图。比如说，日历小部件显示今天的事件；如果用户想要关于一个事件的更多信息，他们可以在小部件中点击事件进入日历app查看它。

`NOTE`  
让用户可以从你的今天小部件打开你的app是很好的，但在小部件中提供有用的，时效性的信息也是必要的。人们不会喜欢唯一功能就是启动一个app的今天小部件。

`必要的话，让人们知道他们需要登录来在你的今天小部件中获取有用的信息。`如果你的今天小部件需要人们登录来查看信息，显示一条信息鼓励他们去登录并解释他们登录后什么内容会显示。比如说，如果你的今天小部件在用户登录后显示即将到来的预定，你可以询问人们去“登录我的app来查看即将到来的预定。”

`不要创建一个启动其他app的今天小部件。`一个模仿iOS主屏幕行为的今天小部件不会提供对你用户有用的功能。

#### 分享和动作扩展
人们通过在一个app中点击动作按钮获取分享和动作扩展。在动作按钮显示的动作视图控制器内，动作扩展会在底部行内列出，分享扩展会在他们上面列出。人么你可以使用更多按钮来管理显示在这个动作视图控制器中的分享和动作扩展。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/3.jpeg)

分享和动作扩展通常使用用户当前环境的内容作为输入。比如在Safari中阅读一篇文章时，用户也许会点击动作按钮并使用分享扩展来将文章发布到一个分享网站或者使用动作扩展来查看文章的翻译。

`NOTE`  
在动作视图控制器中，iOS只会列出支持当前内容类型的动作扩展。比如说当用户当前的内容是一个视频时，iOS不会列出只支持文本的动作扩展。

`尽可能地在分享扩展中使用系统提供的UI。`系统提供的组合视图控制器给予用户一致的体验并且会自动支持一般的任务，例如预览和确认标准内容、同步内容和查看动画以及设置一个发布。查看[App Extension Programming Guide](https://developer.apple.com/library/ios/documentation/General/Conceptual/ExtensibilityPG/index.html#//apple_ref/doc/uid/TP40014214)中的[Share](https://developer.apple.com/library/ios/documentation/General/Conceptual/ExtensibilityPG/ShareSheet.html#//apple_ref/doc/uid/TP40014214-CH12)学习更多关于系统提供的组合视图控制器的使用。

`考虑在一个分享扩展的包容性app中显示一个长上传的进度。`即使分享内容很大，人们也期望在点击一个扩展的发布或分享按钮后能够立即返回到他们原先的环境。你需要让进度是可更新的，但人们不想在每次上传完成时都获得一个通知，而且也没有办法用程序重新启动一个扩展。在这种情况下，在包容性app中显示上传进度就可以了，它能够在后台处理任务，并在有问题的时候发送一个通知。

`为动作扩展使用单色版的app图标。`（相反，分享扩展使用其包容性app的全色图标。）为了创建一个动作扩展的图标，你也许会从创建一个app图标的模板开始。如果必要的话，简化设计并专注于使你的app独一无二的元素。

如果你在你的包容性app中提供多个动作扩展，为他们创建一系列的图标会比较好。确保每一个图标看起来都和app本身的图标相关。

#### 图片编辑扩展
当人们在照片app中浏览照片或者视频时可以使用图片编辑扩展。一般来说，图片编辑扩展帮助用户对一个图片或者视频添加滤镜或者其他编辑。在用户完成更改之后，编辑后的内容可以在照片app中看到。

照片app提供了一个modal视图来显示你的图片编辑扩展的自定义UI。照片app也可以在用户对照片或者视频编辑之后选择取消按钮时显示一个确认视图（你可以在代码中决定是否有这种行为）。

`不要在你的图片编辑扩展中使用导航栏。`正如你在这里看到的一样，封装了你的扩展视图的modal视图已经包含了导航栏；再添加一个导航栏会占据你UI的空间，而且会让你的用户感到困惑。（默认情况下，照片app会以全屏高度显示你的视图，所以你的内容会在内置的导航栏下面。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/4.jpeg)

#### 文档提供扩展
文档提供扩展帮助人们连接你的app管理的包括其他app范围的文档。在许多app中，文档选取视图控制器显示你的扩展提供的UI（查看[UIDocumentPickerViewController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIDocumentPickerViewController_Class/index.html#//apple_ref/doc/uid/TP40014342)学习更多关于文档选取视图控制器的内容）。

`NOTE`  
一个文档提供扩展可以由两个部分组成：一个文档选取视图控制器扩展和一个文件提供扩展。文档选取视图控制器扩展包含了你自定义的UI；而文件提供扩展实现对文件的连接。简单地说，这个章节使用“文档提供扩展”来表示文档选取视图控制器部分提供的UI和体验。

`不要在你的文档提供扩展中使用导航栏。`iOS在文档选取视图控制器内置的导航栏中显示你的扩展自定义的UI。在内置的导航栏下面显示第二个导航栏会让用户感到困惑并且会占据你内容的控件。（默认情况下，文档选取视图控制器使用满屏高度显示你的UI，所以你的内容会在内置的导航栏下方显示。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/5.jpeg)

#### 自定义键盘
人们使用键盘扩展来在全系统使用自定义的键盘代替iOS键盘。在使用键盘扩展后，除了安全文本输入区域（如密码区域）和手机号输入区域（如联系人中的手机号区域）外，人们会在他们点击任何文本输入区域时获取自定义的键盘。

`提供一个明显的方式让用户切换到下一个键盘。`人们对iOS的地球按键很熟悉，并且他们也希望在你的键盘上获得相似的体验。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/App%20Extensions/6.jpeg)

合适的话，在你的包容性app中加入一个教程。必要的话，使用你的自定义键盘的包容性app来给用户一个如何使用你的键盘的说明。不要直接将信息放在键盘内，因为这也许会使人们在尝试使用键盘时感到困惑。

### <a name="HomeKit"/>HomeKit
#### HomeKit智能家居平台
智能家居平台使人们可以方便地在他们的iOS设备上使用家庭自动化app来控制或者设置他们房屋连接的家居，无论配件是哪个厂家的。最好的房屋自动化app整合HomeKit和iOS来帮助用户：
* 建立房屋、房间和空间
* 添加、寻找和移除家居，例如灯泡或恒温控制器
* 定义适用于多个家居的行为
* 管理用户
* 使用Siri来控制他们的房屋

阅读[HomeKit Developer Guide]()https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/HomeKitDeveloperGuide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40015050来学习如何在你的app中使用HomeKit。下面的指南能够帮助你创建一个简单并且乐于使用的房屋自动化app。

`不要假设你的家具是用户安装的第一个家居。`你的app应该让用户创建房屋、房间和空间变得简单，但同样要让用户可以方便地将你的家居安置到已设置好的空间中去。

`让添加新家居变得简单。`不要在用户能够添加家居之前强制用户创建一个账号。你的app最好能偶自动搜索新家居并将它们显著地推送到UI界面中。确保显示关于每个家居足够的信息让用户能够简单地识别它们。

`帮助用户识别他们正在调整的家具。`提供一个帮助用户物理识别家居的控制；比如说，你也许会让用户闪一下灯泡来确认他们是否正在调整他们想要调整的那个灯泡。

`给予用户不同的方式来找到家居。`日期、季节以及用户当前的位置都会影响在给定情况下哪个家居是重要的，所以你的app应该提供一个根据类别、名称或者在房屋中的位置来寻找家居的方式。

`基于在房屋中安装家居的建议操作集。`操作集让用户定义多个家居的独特行为。比如一个“离开”操作集也许会降低房屋的温度、关灯以及锁上所有的门。你的app可以建议预定义的操作集或者让用户创建他们自己的操作集。如果用户能够创建他们自己的操作集，最好让用户从你建议的、基于选择的房间或空间的家具中选择。

使用友好的、会话的语言来使你的app亲切且易于使用。房屋自动化会让用户觉得畏惧。不要使用他们可能不理解的缩略词或者技术术语。尤其HomeKit是一个关于API的技术术语，所以不应该在你的app中使用它。

`NOTE`
如果你是一个方案提供商，浏览方案门户网站获取关于家居包装命名和发送消息的指南。

`整合Siri。`Siri可以使通过简单的语言完成复杂的操作变得简单。Siri能够识别操作集、房屋、房间和空间的名字并且能够理解像“Siri，锁上前门”，“Siri，关掉楼上的灯”以及“Siri，让媒体室暖和一点”的语句。下面的指南可以帮助你给予用户一个非常棒的用户Siri控制他们的家居的体验。
* `使用服务名——而不是家居名——这样Siri就能够识别它。`一个家居可以有多种服务，比如一个有着光服务和风扇服务的吊扇，所以帮助用户区分他们很重要。最好的结果是，让用户从一个有限的名称列表中选择，其不包括公司名、模式数字并且确保让用户在之后编辑名称。你建议的名称应该是描述服务的标准的、易于理解的单词或短语，并且视情况可以包含在房屋中的位置，比如“客厅的灯”或者“车库的门”。你也可以让用户指定输出和开关的服务类型，这样通用的命令如“Siri，关灯”就可以控制所有的灯、照明器具和其他光家居。
* `让用户知道如何在他们设置的时候使用Siri来控制一个操作集。`比如说，当确认“电影”操作集被设置的时候，显示一个用户可以对Siri说的建议的语句，如“你可以通过说‘Siri，将房屋转为电影模式’来使用Siri执行这一操作集”。注意用户也可以简单地说出操作集的名称来告诉Siri执行一个操作集。Siri识别至少设置了一个动作的预定义的和用户定义的操作集。

`帮助用户设置触发器。`在iOS 9中，HomeKit支持触发器，这是一种基于如时间、位置和其他家居的行为的关系条件来执行动作的方式。比如说，用户也许会设置一个触发器在车库门打开并且太阳落山后时打开厨房的灯。设置包含多个条目的关系条件会变得混乱，所以使设置UI尽可能的简单很重要。比如说，在一个反应人们所说的内容的命令中显示条目、属性和逻辑操作会帮助用户理解情况。

### <a name="Multitasking"/>Multitasking
#### 多任务处理
多任务处理让人们在屏幕上（以及合适的iPad模式）查看多个app，并且在最近使用的app中快速地切换。在iOS 9中，人们可以使用多任务处理UI（如下所示）来选择一个最近使用的app。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Multitasking/1.jpeg)

在多任务处理环境中的成功取决于与设备上其他app的和谐共处。在高层面上，这意味着app应该：
* 用心地优化资源的使用来避免使用过多的CPU、内存、屏幕控件和其他资源
* 优雅地处理其他app的干扰和声音
* 停止和重新开始——即过渡到后台或从后台过渡——快速而平滑
* 当没有在前台时对行为负责

下面的特有的指南会帮助你的app在多任务处理环境中专注于app切换获取成功。查看[Adopting Multitasking Enhancements on iPad](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/AdoptingMultitaskingOniPad/index.html#//apple_ref/doc/uid/TP40015145)获取更多关于在iPad多任务处理环境下运行的信息。

`准备好被打断和继续。`多任务增加了后台app打断你的app的可能性。其他的特性例如推送广告和快速app切换也会导致更高频率的打断。你越快越准确地保存你app当前的状态，人们就能越快地重新启动并继续他们离开时的工作。为了给予用户一种无缝重启的体验，利用UIKist的保存和恢复功能（查看[Preserving Your App’s Visual Appearance Across Launches](https://developer.apple.com/library/ios/documentation/iPhone/Conceptual/iPhoneOSProgrammingGuide/StrategiesforImplementingYourApp/StrategiesforImplementingYourApp.html#//apple_ref/doc/uid/TP40007072-CH5-SW2)获取更多信息）。

`确保你的UI能够处理两层高度的状态栏。`两层高度状态栏在例如进程中来电、语音录制和共享数据。在没准备的app中状态栏额外的高度会导致布局的问题。比如说，UI会变低或者被覆盖住。在多任务处理环境中，能够处理两层高度的状态栏尤其重要，因为有更多的app会导致其出现。

`准备好暂停需要人们关注或者参与的活动。`比如说，如果你的app是一个游戏或者播放视频的app，确保用户切换离开你的app时不会错过任何内容或事件。当人们切换回一个游戏或者视频播放器，他们想要像从没离开过一样继续体验。

`确保你的声音表现得体。`多任务处理使得你的app在运行时更有可能发生别的多媒体活动。因此你的声音也更有可能不得不暂停和重新开始来处理中断。查看[Sound](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Sound.html#//apple_ref/doc/uid/TP40006556-CH44-SW1)来获取指南帮助你确保你的声音符合人们的预期并且和设备上的其他声音和谐共存。

`有节制地使用本地通知。`一个app可以安排在特定的时间发送本地通知，无论这个app是挂起、在后台运行还是没有运行。为了达到最好的用户体验，避免用过多的通知纠缠人们，并且遵循[Notifications](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/NotificationCenter.html#//apple_ref/doc/uid/TP40006556-CH39-SW1)中描述的创建通知内容的指南。

`合适的时候结束后台用户发起的任务。`当人们发起一个任务，他们通常期望它即使在切换离开app时也能结束。如果你的app正在执行一个用户发起的不需要用户额外交互的任务，你应该在挂起前在后台完成它。

### <a name="Notifications"/>Notifications
#### 通知
通知给予人们当前重要的信息和功能。人们可以从很多环境下得到通知，比如锁屏上、使用app时以及浏览通知中心时。

通知中心有两个视图：今天和通知。

今天视图显示一个可编辑的小部件列表。今天小部件是一个显示由用户关心的app提供的少量即时的、高价值的信息或功能的app扩展。比如说，日历小部件只显示今天的事件。在日历小部件中点击一个事件会在日历app中打开此事件，从而允许用户编辑此事件以及管理其他事件。查看App Extensions学习更多关于设计今天小部件的内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/1.jpeg)

通知视图显示用户感兴趣的app的最近的通知信息。用户可以在设置中的app区域指定是否允许app的通知显示在通知中心。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/2.jpeg)

iOS app可以使用通知在有兴趣的事情发生时让人们知晓，比如：
* 收到一个信息
* 一个事件即将发生
* 新数据可以下载
* 某事的状态更改了

在iOS 8以及之后的版本中，app可以定义用户与通知交互的动作。比如说，一个to-do app的通知可以让用户不比打开app就可以标记一个条目为done。

iOS定义了两种通知类型。
* 本地通知是在同一个设备上由app预定，由iOS发送的，无论app当前是否在前台运行。比如说，一个日历或to-do app可以预定一个本地通知来提示人们一个即将到来的会面或者到期时间。
* 远程通知（也称推送通知）是由app的远程服务器推送到苹果的推送通知服务的，会将通知推送到所有安装了app的设备上。比如说，一个用户可以与远程对手对战的游戏会更新所有玩家最近的移动。

`NOTE`
app扩展也许会要求远程通知发送到它的包容性app中去。在这个情况下，包容性app一般会在后台启动来处理通知。查看App Extensions来学习更多关于app扩展的内容。

为了确保用户可以自定义他们的通知体验，你应该尽可能多地支持下面这些通知种类：
* 横幅
* 警告
* 标记
* 声音

`NOTE`  
在iOS 8以及之后的版本中，你必须注册你想要发送给用户的通知类别。你第一次执行注册动作时，用户会得到一个警告来决定他们是否要允许你的app发送通知。无论他们选择什么，用户都可以查看你app的设置来更改这个特性或者指定他们想要接收的通知类型。

横幅是一个小的半透明视图，会在屏幕上显示然后几秒后消失。用户也可以在锁屏界面和通知中心的通知视图看到横幅的其他版本。在横幅中，iOS显示你的通知信息和小的app图标（查看[App Icon](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/AppIcons.html#//apple_ref/doc/uid/TP40006556-CH19-SW1)学习更多关于小图标的内容）。用户点击横幅来清除它并跳转到发送通知的app。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/3.jpeg)

除了默认的点击横幅动作，你还可以定义两个当用户滑动横幅时显示的动作。点击通知动作按钮消除横幅并启动你的app（可能在后台）来处理动作。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/4.jpeg)

通知警告框是一个标准的显示在屏幕上且需要用户交互才能消除的警告视图。你可以提供通知信息以及一个默认的动作或者最多四个在用户点击Options按钮时显示的特殊动作。你无法控制警告框的背景样式。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/5.jpeg)

当用户点击警告框上默认的或者自定义的按钮时，iOS会同时消除警告框并启动你的app（可能在后台）。点击Close或OK按钮会消除警告框而不打开你的app。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/6.jpeg)

标记是一个小红圆，上面显示待查看的通知条目数量（标记显示在app图标的右上角）。你无法控制标记的尺寸以及颜色。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Notifications/7.jpeg)

自定义的或系统提供的声音可以伴随任意其他三种通知类型出现。

`在使用通知中的干扰动作时要三思。`你要确保用户有足够的环境避免意外的影响。为了帮助用户区分你特定的破坏性动作，iOS会用红色显示它。在一些情况下，你的app在执行破坏性的动作前要求用户确认是个好主意。比如说，如果你提供一个显示在锁屏上的横幅中的破坏性动作，你会想要确保只有设备的拥有者可以执行动作（你要在代码中实现这个需求）。

`为每一个动作按钮提供一个自定义的标题。`创建一个简单的标题来清晰地描述发生的动作。比如说，一个游戏也许会使用标题“Play”来表明点击按钮会打开app进入一个地方让用户开始他们的历程。确保标题：
* 使用大写风格的标题
* 足够短来适应按钮而不被截断（确保测试国际化标题的长度）

`不要为同一个事件发送多个通知。`用户在选择通知条目的时候需要专心查看；直到用户以某种方式处理通知条目时它们才会消失。如果你对同一个事件发送多个通知，你会填满通知中心，而且用户可能会关闭你app的通知。

`不要在通知信息中包含你的app名称。`你自定义的信息会在警告框和横幅以及通知中心的通知视图中显示。因为iOS会自动在你的信息中显示你的app名称，所以你不会想在自定义的信息中包含你的app名称。

为了实用，一个本地或远程通知信息应该：
* 专注于信息，而不是用户的动作。不要告诉用户点击哪个警告按钮或者如何打开你的app。
* 足够短到再一两行内显示。长信息对用户来说很难快速阅读，并且这会强制警告框滚动。
* 使用句子风格的大写并且使用合适的标点符号来结束。可能的话，使用一个完整的句子。

`NOTE`  
必要的话iOS会截断你的信息来适应每个通知风格；为了最好的结果，你不应该截断你的信息。

`保持标记的内容更新。`当用户查看新信息后更新标记非常重要，这样他们就不会认为收到了新的通知。注意设置标记内容为0时也会移除通知中心中相关的通知条目。

`IMPORTANT`  
不要以通知以外的目的使用标记。记住用户可以关闭你app的标记，所以你不能确保他们会查看标记的内容。

`提供一个用户可选的收到通知时的声音。`声音可以在人们没有查看设备屏幕时吸引他们的注意。比如说，一个日历app也许会播放一个声音和一个警告框来提醒人们一个即将到来的事件。或者，一个协作任务管理app也许会播放一个声音和一个标记来表示一个远方的同事完成了一个任务。

你可以提供一个自定义的声音，或者你可以使用内置的警告声音。如果你创建自定义的声音，确保它简短、有区分性且为专业产品。（查看[Preparing Custom Alert Sounds](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/Chapters/IPhoneOSClientImp.html#//apple_ref/doc/uid/TP40008194-CH103-SW6)来学习这个声音需要的技术。）注意你不能程序上设置通知到达时使设备震动，因为用户会控制警告是否会伴随震动。

### <a name="Social Media"/>Social Media
#### 社交媒体
人们期待无论他们当前在什么环境下都可以链接到他们最喜欢的社交媒体账户。iOS使以人们赞赏的方式整合社交媒体的交互到你的app中变得简单。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Social%20Media/1.jpeg)

`NOTE`
当用户点击动作按钮时，他们会获取到一个类似这里展示的活动视图控制器。查看[Activity View Controller](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW121)学习更多关于这个视图控制器的内容。
活动视图控制器列表的中间行显示了用户允许的分享app扩展以及系统提供的分享服务。查看[Share and Action Extensions](http://blog.csdn.net/cloudox_/article/details/50392075)学习更多关于设计分享扩展的内容。

`考虑给予用户一个便利的方式来用你的app发布内容。`用户会允许分享扩展来便于在任何地方发布内容，但你也可以使用系统提供的写作视图控制器来给用户一个可以编辑发布内容的视图。你可以选择在你给用户编辑之前预先填充自定义的内容（当你展示给用户编辑视图之后，只有用户可以编辑内容）。查看[Social Framework Reference](https://developer.apple.com/library/ios/documentation/Social/Reference/Social_Framework/index.html#//apple_ref/doc/uid/TP40012233)学习关于社交框架的变成接口——包括[SLComposeViewController](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Reference/SLComposeViewController_Class/index.html#//apple_ref/occ/cl/SLComposeViewController)。

`可能的话，不要要求用户登录一个社交媒体账户。`社交框架回合账号框架协同工作来支持单次登录，所以你可以获得链接到用户的账户的授权。如果用户当前没有登录账户，你可以展示UI让他们去登录。

### <a name="iCloud"/>iCloud
iCloud让人们无论当前使用的是哪个设备都能连接到他们关心的内容。当你整合iCloud到你的app中时，用户就可以使用不同设备上你的app实例来查看和编辑他们的个人内容而不用执行显式的同步。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/iCloud/1.jpeg)

为了提供这个用户体验，很可能你需要重新审核你存储、连接和退信信息的方式——特别是用户创造的内容——在你的app中。查看[iCloud Design Guide](https://developer.apple.com/library/ios/documentation/General/Conceptual/iCloudDesignGuide/Chapters/Introduction.html#//apple_ref/doc/uid/TP40012094)学习如何在你的app中使用iCloud。

iCloud用户体验中一个很基本的方面是透明度：理念上，用户不需要知道他们的内容在何处，并且他们应该很少需要思考他们正在看的是哪个版本的内容。下面的指南可以帮助你给用户他们期待的iCloud体验。

`合适的话，让用户允许你的app使用iCloud变得简单。`在他们的iOS设备上，用户在iCloud设置中登录他们的iCloud账户，而且在大部分情况下，他们希望他们的app自动与iCloud协作。但如果你觉得用户也许会想要选择是否对你的app使用iCloud，你可以在用户第一次打开你的app的时候提供一个简单的选项。在大部分情况下，这个选项应该提供一个关于是否对用户连接的app的所有内容使用iCloud的选择。

`尊重用户的iCloud空间。`记住iCloud是用户购买的有限资源很重要。你应该使用iCloud存储用户创建和理解的信息，而要避免使用它来存储你可以重新生成的app资源和内容。同样，注意当用户的iCloud账户是活动的时，iCloud会自动支持你app文档文件夹的内容。为了避免使用太多用户的空间，你最好对放置在文档文件夹中的内容进行筛选。

`决定存储在iCloud中的信息类型。`为了存储用户创建的文件和其他内容，你也可以存储少量的数据比如用户当前在你app中的状态或者他们的偏好。使用iCloud键值对仓库存储这种类型的信息。比如说，如果人们使用你的app来阅读一本杂志，你也许会使用iCloud键值对存储他们最新阅读的页面，这样当他们在一个不同的设备上再次打开时，他们可以从他们离开的地方继续阅读。

如果你使用iCloud键值对仓库存储偏好，确保这个偏好是用户想要在所有他们的设备上使用的。比如说，有些偏好在工作环境下比在家庭环境下更加有用。在一些情况下，将偏好存储在你app的服务器上而不是用户的iCloud账户上会更有意义，这样无论iCloud是否被使用，偏好都会起作用。

`确保你的app在iCloud不被使用时行为合理。`比如说，如果用户注销了他们的iCloud账户，就关闭iCloud在你app中的使用，或者进入飞行模式时，iCloud也会变得无法使用。在这些情况下，用户执行一个关闭连接iCloud的动作，所以你的app不需要告诉他们这件事。不过，告诉用户他们做出的更改知道他们重新连接到iCloud之前不会在他们的其他设备上显示会比较好。

`不要给予用户选项来创建本地文件。`无论你是否在你的app中支持iCloud，你都不应该鼓励用户去思考一个设备独有的文件系统。相反，你想要用户专注于通过iCloud使他们的内容具有普遍可用性。

`合适的话，自动更新内容。`最好不需要用户做任何事就可以确保他们获取到了你app中最新的内容。不过你需要平衡这个体验和用户的设备空间与带宽限制。如果你的用户工作处理非常大的文档，给予他们一个关于是否从iCloud下载更新的控制会比较好。如果你需要这样做，设计一个方式来表示在iCloud中有一个最近的文档版本可以获取。当用户选择更新文档时，如果下载花费很多时间，确保提供一个反馈。

`警告用户删除一个文档的后果。`当用户在一个使用iCloud的app中删除一个文档时，文档会在用户的iCloud账户和所有其他设备中移除。在执行删除之前显示一个警告框来描述这个结果并获取确认会比较好。

`尽快地告知用户冲突，但只在必要的时候告知。`使用iCloud编程接口，你应该能够解决一个文档不同版本之间的大部分冲突而不影响用户。如果有不能解决的，确保你尽快地发现冲突这样就可以帮助用户避免浪费时间在错误的内容版本上。你需要设计一个不唐突的方式来告诉用户存在一个冲突；然后让用户能够简单地区分版本并且做出决定。

`确保在搜索时包含用户iCloud的内容。`使用iCloud账户的用户倾向于认为他们的内容是一个可获取的整体，并且他们希望搜索结果可以反映这一观点。如果你的app允许用户搜索他们的内容，确保你使用合适的API来扩展搜索到他们iCloud的账户

### <a name="HealthKit"/>HealthKit
在iOS 8以及之后的系统中，整合HealthKit的app可以从健康app中获取数据来提供更加强大和全面的健康和健身服务。获取用户许可后，app可以从健康app（用户健康相关数据的存储中心）获取HealthKit的读写数据权限。

比如说，用户可以允许一个营养app获取他们存储在健康app的体重和活动数据，这样营养app就可以推荐每日的卡路里消耗量来达到某个明确的目标。这个营养app也可以使用HealthKit来更新健康app中实际消耗的卡路里量，这样用户可以更简单地跟踪他们的进度，查看[HealthKit Framework Reference](https://developer.apple.com/library/ios/documentation/HealthKit/Reference/HealthKit_Framework/index.html#//apple_ref/doc/uid/TP40014707)学习如何整合HealthKit到你的app。

下面的指南可以帮助你创建一个人们信任并享受使用的健康和健身app。

`只在你有迫不得已的原因时去请求获取健康数据。`HealthKit是设计为专注于健康和健身服务的app使用的。如果一个app要求获取不相关的健康信息，用户不太可能信任使用他们私有数据的app。所以你要确保用户理解你的app需要链接到他们某些私人健康数据并从分享数据中获益。

`不要在用户有机会理解健康数据用来做什么时请求健康数据。`人们倾向于在他们看到他们当前的任务和你请求数据之间的关联时给予他们健康数据的链接。比如说，当用户填写一个减肥app的基本信息时，请求获取他们存储在健康app中的体重数据就有意义。但如果这个减肥app在app启动时立马请求链接体重数据，用户可能不太愿意分享他们的私人信息。

`使用系统提供的UI来请求获取用户的数据。`用户期待在他们需要授予链接他们数据的许可时立马看到如下所示系统提供的许可表单。为了提供一个好的用户体验，不要再你app的其他界面重复许可表单的信息。相反，你可以在许可表单中添加自定义的信息来解释为什么你的app需要链接某些数据（查看[HKHealthStore Class Reference](https://developer.apple.com/library/ios/documentation/HealthKit/Reference/HKHealthStore_Class/index.html#//apple_ref/doc/uid/TP40014708)获取更多信息）。保持这些信息简洁，但确保它们清晰地传达了你的app如何使用健康数据以及分享数据的好处。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/HealthKit/1.jpeg)

`NOTE`
如果用户决定停止分享数据到你的app，他们会在设置中做出这个修改。不需要在你app的UI中添加这个功能。

`不要在你的UI中使用健康app图标、图片或者截屏。`对于所有的苹果设计，这些图片都是有版权的并且不应该被显示在你的app中。

`不要在你的UI中使用“HealthKit”的术语。`HealthKit是一个开发术语，表示你链接存储在健康app中的数据的技术框架。如果你需要涉及你的app与存储在健康app中的数据协同工作的方式，使用术语“健康app”。比如说，你可以说你的app“存储信息到健康app中”或“使用从健康app中获取的数据”。

### <a name="In-App Purchase"/>In-App Purchase
#### app内购买
app内购买让人们在你的app中你设计的商店购买数字产品。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/In-App%20Purchase/1.jpeg)

比如说，用户也许会：
* 从一个基本版app升级到一个付费版
* 为新的每月内容续费
* 购买虚拟条目，比如一个游戏中的新等级或武器
* 购买和下载新的书籍

使用StoreKit框架来将商店嵌入到你的app中并支持app内购买。当一个用户做出一次购买时，StoreKit连接App Store来安全地执行支付，然后通知你的app，这样就可以提供购买条目。

`IMPORTANT`
app内购买只汇集支付——你要提供额外的功能，比如将你的商店展现给用户，解锁内置的特性，以及从你的服务器下载内容。还有，所有你通过app内购买销售的产品都必须在App Store注册。
查看[In-App Purchase Programming Guide](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/StoreKitGuide/Introduction.html#//apple_ref/doc/uid/TP40008267)学习添加商店到你的app的技术需求。查看[App Store Resource Center](https://developer.apple.com/app-store/)获取更多使用app内购买的商务需求的信息。你也应该阅读关于你可能销售的和你如何在app中提供这些产品的明确的许可协议信息。

下面的指南可以帮助你设计一个用户喜欢的购买体验。

`优雅地整合商店体验到你的app中。`当展示商品和处理用户的事务时，在你的app中创建一种宾至如归的体验。你不会希望当用户浏览你的商店时感觉进入到了一个不同的app。

`使用简洁的标题和描述。`最好人们可以浏览一系列条目然后快速地找到他们感兴趣的内容。当你使用简单直观而不冗杂的语言和标题时，人们就可以简单地理解你提供的商品。

`不要更改默认的确认警告框。`当用户购买一个商品时，StoreKit会显示一个确认警告框（如上所示）。你不应该修改这个警告框，因为它可以帮助用户避免意外的购买。

### <a name="Game Center"/>Game Center
#### 游戏中心
游戏中心可以让人们玩游戏、组织在线多人游戏以及其他功能。玩家使用内置的游戏中心app来登录一个账号、发现新游戏、添加新朋友、浏览排行榜和成就。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Game%20Center/1.jpeg)

作为一个游戏开发者，你使用GameKit API来传递分数和成就到游戏中心服务、在游戏的UI中显示排行榜、以及帮助用户找到其他的玩家。查看[Game Center Programming Guide](https://developer.apple.com/library/ios/documentation/NetworkingInternet/Conceptual/GameKit_Guide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40008304)来学习如何整合游戏中心到你的app中去。

下面的指南可以帮助你在你的app中给用户一个好的游戏中心体验。

`不要创建自定义的UI提示用户从游戏中心登录。`当人们启动你的允许使用游戏中心的app时——并且他们没有在他们设备上的游戏中心登录——系统会自动提示他们登录。显示自定义的UI是不必要的，而且可能导致用户迷惑。

`一般来说，使用标准的游戏中心UI。`很少情况下，自定义游戏中心的UI会有意义，但这么做会迷惑人们。标准的游戏中心UI——iOS和OS X的用户都很熟悉——会提升属于一个大的游戏社区的感觉。

`让用户可以关闭语音聊天。`一些用户在开始游戏时可能不会想要自动打开语音聊天，并且大部分用户会感激在特定情况下关闭语音聊天的能力。

### <a name="iAd Rich Media Ads"/>iAd Rich Media Ads
#### iAd富媒体广告
当你允许广告在你的app中出现时，用户查看或与它们交互时你可以得到收入。（这里你可以看到一个简单的工程中iAd横幅的占位符。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/iAd%20Rich%20Media%20Ads/1.jpeg)

你在你UI的一个特定的视图中展示一个iAd网络服务的广告。首先，这个视图可以包含广告的横幅，用来进入完整的iAd体验。当人们点击横幅时，广告执行一个事先确定的动作，比如播放一个视频、显示交互内容、或者启动Safari来打开一个网页。这个动作可以覆盖你的UI来显示内容，或者让你的app切换到后台。

有三种类型的横幅可以用来显示在你的app中：标准型、中型矩形和全屏型。所有类型的横幅服务于同一个目标——即引导用户进入广告——但他们在表现形式和行为上不同。

标准横幅占用屏幕的一小块区域，并且往往会始终存在屏幕中。你可以选择应该显示标准横幅的app界面并且在布局中留出放置横幅视图的空间。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/iAd%20Rich%20Media%20Ads/2.jpeg)

所有的iOS app都可以显示标准横幅。使用[ADBannerView](https://developer.apple.com/library/ios/documentation/UserExperience/Reference/ADBannerView_Ref/index.html#//apple_ref/occ/cl/ADBannerView)类提供的视图去在你的app中包含标准横幅。

中型矩形横幅和标准横幅的行为类似，你选择应该在何处放置中型矩形横幅。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/iAd%20Rich%20Media%20Ads/3.jpeg)

中型矩形横幅只能在iPad app中使用。使用[ADBannerView](https://developer.apple.com/library/ios/documentation/UserExperience/Reference/ADBannerView_Ref/index.html#//apple_ref/occ/cl/ADBannerView)类提供的视图在你的app中包含中型矩形横幅。

全屏横幅占用大部分或全部的屏幕，并且通常在特定的位置特定的时间出现。你可以选择是模态地显示横幅还是在一个可滚动内容的分开的页面显示。（在这里显示的例子中，app提供一个杂志阅读体验并且让用户可以在全屏横幅上翻页。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/iAd%20Rich%20Media%20Ads/4.jpeg)

使用[ADInterstitialAd](https://developer.apple.com/library/ios/documentation/iAd/Reference/ADInterstitialAd_Ref/index.html#//apple_ref/occ/cl/ADInterstitialAd)类提供的视图来在你的app中包含全屏横幅。

所有的横幅都在iAd框架中显示，会在右下角显示iAd的标识。iAd框架被设计成固定在你的app屏幕底部边缘时最好看的样子。

为了确保和横幅广告的无缝交互并提供最好的用户体验，请遵循下面的指南。

`将标准横幅放置在屏幕的底部或者靠近底部。`这个位置略有不同，取决于在屏幕底部是否有栏以及是什么类型的栏。

栏 | 标准横幅视图的位置
---|---
在屏幕底部没有栏 | 放置在屏幕底部
在屏幕的任何位置都没有栏 | 放置在屏幕底部
工具栏或者标签栏 | 放置在在底部栏的上方

`在不会干扰到用户内容的地方放置中型矩形横幅视图。`和标准视图一样，中型横幅同样在屏幕的底部或靠近底部是最好的。将横幅放置在靠近屏幕底部的地方也可以增加不影响用户的可能性。

`当在用户体验中有穿插的时候模态地展示全屏横幅。`如果在你app的流程中有自然的中断和环境改变，模态展示风格是比较好的。当你模态地展示全屏横幅时（通过使用[presentFromViewController:](https://developer.apple.com/library/ios/documentation/iAd/Reference/ADInterstitialAd_Ref/index.html#//apple_ref/occ/instm/ADInterstitialAd/presentFromViewController:)），用户一定会进入广告或者消除它。由于这个理由，当用户期待体验的改变时使用模态展示风格是个好主意，比如在他们完成一个任务之后。

`当用户在app视图间过渡时非模态地展示全屏横幅。`如果用户频繁地过渡屏幕来体验你的app，比如在一个杂志中翻页或者轻拂一系列条目，非模态的展示风格会比较好。当你非模态地展示一个全屏横幅时（通过使用[presentInView:](https://developer.apple.com/library/ios/documentation/iAd/Reference/ADInterstitialAd_Ref/index.html#//apple_ref/occ/instm/ADInterstitialAd/presentInView:)），你可以保存你UI中的栏，这样用户就可以使用app的控制来跳过或者回到广告。和所有横幅一样，当用户点击全屏横幅时会启动一个iAd体验，但你的app可以在合适的情况下响应横幅区域上的其他手势（比如拖拽或者滑动）。

确保使用合适的动画来显示和隐藏非模态的全屏横幅视图。比如说，一个杂志阅读app可能会用显示其他内容页面的翻页动画来显示一个横幅。

`确保所有横幅在你app中有意义的时间和地方显示。`人们倾向于在不觉得干扰了他们工作流的时候进入一个iAd体验。在沉浸式app比如游戏中这一点尤其重要：你不会想要在会与玩游戏相冲突的地方放置横幅视图。

`不要在用户只想短暂地查看的界面显示横幅。`如果你的app包含那些用户为了进入到他们关心的内容而快速跳转的界面，最好不要在这些界面显示横幅。用户倾向于在停留于界面超过一两秒时点击横幅。

`尽可能地在各个方向显示横幅。`用户最好不需要在改变设备方向时从使用你的app和查看广告之间切换。同样的，支持各个方向会让你能接受更大范围的广告。查看[iAd Programming Guide](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/iAd_Guide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40009881)学习如何确保横幅视图响应方向的更改。

`不要让标准横幅和中型矩形横幅滚动出屏幕。`如果你的app在屏幕上显示滚动内容，确保横幅视图保持固定在其位置。

`当人们查看或与广告交互时，暂停需要他们关注和交互的活动。`当用户选择查看一个广告时，他们不想觉得他们错过了你app的事件，并且他们不希望你的app打断广告的体验。好的做法是停止那些当你的app过渡到后台时停止的活动。

`不要停止一个广告，在罕见的情况下除外。`一般来说，在用户查看和与广告交互时，你的app会持续运行和接收事件，所有可能有的事件会发生并且急需他们立即关注。然而很少有情况需要停止一个进行中的广告。一种可能性是一个提供网络电话（VoIP）的app。在这种app中，当一个电话打过来时取消一个运行的广告可能是有意义的。

`NOTE`
取消一个广告可能对你的app能够接收的广告和你的收入带来不利的影响。

### <a name="AirPrint"/>AirPrint
#### 无线打印
使用AirPrint无线打印，人们可以从你的app无线地打印内容并使用打印中心app来检查打印工作。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/AirPrint/1.jpeg)

你可以得益于内置的对打印图片和PDF内容的支持，或者你可以使用打印编程接口自定义格式和渲染。iOS会处理打印机的发现和所选择的打印机的打印工作的调度与执行。

一般来说，当用户想要打印一些东西的时候会点击你app中的标准动作按钮。当他们在显示的视图上选择打印条目后，他们可以选择一个打印机，设置打印选项，并点击打印按钮来开始打印。

用户可以在打印中心app检查他们请求的打印工作，这是一个只有在有打印工作在进程中时才可以获取的后台系统app。在打印中心中，用户可以查看当前的打印队列，获取一个特定打印工作的详情以及取消工作。

你可以在你的app中添加相对少量的代码来支持基本的打印（查看[Drawing and Printing Guide for iOS](https://developer.apple.com/library/ios/documentation/2DDrawing/Conceptual/DrawingPrintingiOS/Introduction/Introduction.html#//apple_ref/doc/uid/TP40010156)学习关于在你的代码中添加打印支持的内容）。为了确保用户喜欢你app的打印体验，遵循下面的指南：

`使用系统提供的动作按钮。`用户对这个按钮的意义和行为很熟悉，所以可能的话使用它是一个好主意。除非你的app不包含工具栏或者导航栏。在这种情况下，你需要设计一个自定义的打印按钮显示在你app的主UI中，因为这个动作按钮只能在工具栏和导航栏使用。

`当打印是当前环境的主要功能时显示打印条目。`如果打印对当前环境不合适，或者如果用户不想要打印，不要在动作按钮显示的视图中包含打印条目。

`合适的话，提供额外的打印选项给用户。`比如说，你可能会允许用户来选择一个页面范围或者要求打印多份。

`如果用户无法打印，不要显示打印细节。`在你显示可以选择打印的UI前，确保用户的设备是否支持打印。查看[UIPrintInteractionController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIPrintInteractionController_Class/index.html#//apple_ref/doc/uid/TP40010141)学习如何在你的代码中这样做。

### <a name="Accessing User Data"/>Accessing User Data
#### 访问用户数据
定位服务允许app来确定人们大致的地理位置、他们设备指向的方向以及他们移动的方向。其他系统服务——诸如联系人、日历、提醒以及相册——也允许app去访问用户存储在其中的数据。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Accessing%20User%20Data/1.jpeg)

即使人们喜爱app知道很多他们的信息带来的便利性，他们也会希望能够选择保护他们数据的隐私性。比如说，人们喜欢能够自动标记他们的物理位置或者寻找附近的朋友，但他们也希望在他们选择不分享他们的位置给别人时能够禁用这些特性。（查看[Location and Maps Programming Guide](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/LocationAwarenessPG/Introduction/Introduction.html#//apple_ref/doc/uid/TP40009497)学习更多关于如何让你的app定位的内容。）

下面的指南可以帮助你以用户感到舒适的方式获取到用户数据。

`确保用户理解为什么他们被询问分享他们的私人数据。`如果人们没有看到一个明显的数据需要，他们很自然地会对索取他们的私人信息感到怀疑。为了避免让用户不舒服，确保只在他们尝试使用清晰地需要知道他们的信息的特性时显示警告框。比如说，人们可以再定位服务关闭时使用地图，但是在他们使用寻找和跟踪他们当前位置的特性时会看到一个警告框。

`如果不明显的话，描述为何你的app需要信息。`你可以提供显示在警告框中的文本，放在系统提供的诸如“‘App 名’想要使用您的联系人”或者对于定位通知，“允许‘App 名’在你使用app的时候使用你的位置么？”的标题下面。你会想要这个文本明确而礼貌，这样人们就会理解为什么你要求连接他们的信息，并且不会感到压力。

你的理由文本应该：
* 不包含你的app名。系统提供的警告标题已经包含了你的app名。
* 清晰地描述为什么你的app需要这个数据。合适的话，你也可以解释不适用数据时你app的方式。
* 使用以用户为中心的术语并且局部化。
* 尽可能地简短，但依然易于理解。尽可能地不要超过一句话。
* 使用句子风格的大写。（句子风格的大写指第一个字母是大写的，其他字母都是小写的，除非是专有名词和专有形容词。）

`只有当你的app没有用户数据无法执行主要功能时才在启动app时请求数据许可。`如果很明显你app的主要功能依赖于知晓人们的私人数据，他们就不会感到烦恼。

不要在用户选择需要数据的特性之前编程触发警告框。这样，你就可以避免在用户做不需要数据的事情时让他们纳闷为什么你的app想要他们的私人数据。（注意检查用户的定位服务偏好不会出发警告框。）

`对于位置数据，检查定位服务的偏好避免不必要地触发警告框。`你可以使用Core Location编程接口获取这个设置（查看[Core Location Framework Reference](https://developer.apple.com/library/ios/documentation/CoreLocation/Reference/CoreLocation_Framework/index.html#//apple_ref/doc/uid/TP40007123)学习如何做）。有了这个知识，你就可以尽可能地在请求位置信息时触发警告框，或者可能完全不要警告框。

### <a name="Quick Look"/>Quick Look
#### 快速浏览
使用快速浏览，即使你的app不能打开文档，用户也可以通过你的app预览一个文档。比如说，你也许会允许用户预览他们从网页下载或者从其他资源获取的文档。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Quick%20Look/1.jpeg)

查看[Document Interaction Programming Topics for iOS](https://developer.apple.com/library/ios/documentation/FileManagement/Conceptual/DocumentInteraction_TopicsForIOS/Introduction/Introduction.html#//apple_ref/doc/uid/TP40010403)学习更多关于如何在你的app支持快速浏览文档预览的内容。

在用户从你的app预览一个文档之前，他们可以在你创建的自定义视图查看文档的信息。比如说，用户下载了一封邮件附件的文档之后，邮件会在自定义的视图显示一个文档的图标、标题和大小。用户可以点击这个视图来预览文档。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Quick%20Look/2.jpeg)

你可以在你的app中显示一个新视图来展示文档，或者在一个全屏的模态视图中展示。展示的方法取决于你app运行的设备。

`在iPad上，模态地显示一个文档预览。`iPad的大屏幕很适合在一个沉浸式的环境中显示一个文档预览让用户可以很容易地离开。空间过渡尤其适合显示预览。

`在iPhone上，在一个专门的视图上，导航视图更好，来显示文档预览。`这样做让用户可以不丢失你app的上下文来导航到文档预览或者从文档预览导航出去。虽然也可以在iPhone app中模态地显示文档预览，但并不推荐这样做。（注意空间过渡并不适用于iPhone.）

还有要注意，在导航视图显示文档预览让快速浏览可以在导航栏上放置预览导航控件。（如果你的视图已经包含工具栏，快速浏览会在工具栏放置预览导航控件。）

### <a name="Sound"/>Sound
#### 声音
无论声音是你app用户体验的主要部分还是一个可选的增益，你都要知道用户对声音有何期待以及如何满足这些期待。

#### 理解用户的期待
用户可以使用设备的控制来影响声音，并且他们可能使用有线或无线的耳机。人们也对他们的行为如何影响他们听到的声音抱有很多期待。虽然你可能会发现有些期待很惊人，但这都遵循用户，而不是设备，决定的用户控制。

当用户想要做如下事情的时候他们会使设备静音：
* 避免被不期待的声音干扰，比如电话铃声和收到短信的声音
* 避免听到用户行为副产品的声音，比如键盘或其他反馈声音、附带声音或者app启动声音
* 避免听到对使用游戏非必要的游戏声音，比如音效和配乐

比如说，在电影院内用户使他们的设备静音避免打扰到其他的人。在这种情况下，用户依然想要在他们的设备上使用app，但不想被他们不期待或者请求明显的声音所惊吓，比如铃声或者新短信声。

静音开关不会关闭单独由用户动作导致的和明确为了产生声音的声音。比如：
* 一个只播放媒体的app中的媒体播放不会被静音，因为媒体播放是明确被用户请求的。
* 闹钟不会被静音，因为闹钟是明确被用户设置的。
* 语言学习app中的音效素材不会被静音，因为用户明确要听到它。
* 语音聊天app中的对话不会被静音，因为用户启动app的唯一目的就是进行语音聊天。

`用户使用设备的音量按钮来调整他们设备可以播放的所有声音的音量，`包括歌曲、app声音和设备声音。无论静音开关的位置在哪，用户都可以使用音量按钮来安静任何声音。使用音量按钮来调整一个app当前播放的音量同样会调整所有系统的音量，包括铃声音量。

`IPHONE`
当没有声音播放时使用音量按钮会调整铃声音量。

`用户使用耳机来私下听声音并解放他们的双手。`无论这些设备是有线的还是无线的，用户都有着特殊的用户体验的期待。

当用户插上耳机，或者连接到一个无线声音设备时，他们想要继续听到当前的声音，但是是私下的。因此，他们希望当前正在播放声音的app能够不暂停地继续播放。

当用户拔出耳机，或者从一个无线设备断开连接（或者设备超出距离或者关闭）时，他们不想自动分享他们听的内容给其他人。因此他们希望当前正在播放声音的app暂停，允许他们在准备好的时候重新播放。

#### 定义你app的声音行为
`如果有必要，你可以对你的app调整相关的，独立的音量水平来产生最好的混合音频输出。`但最终输出的音量应该总是由系统音量所管理，无论是音量按钮还是音量滑动条。这意味着app的声音输出依然由所属的用户来掌控。

`合适的话，确保你的app可以选择音频线路。`（音频线路指声音信号的一个电子线路，例如从设备到耳机或者从设备到话筒。）即使人们不物理地插上或者拔出无线声音设备，他们也希望能够选择一个不同的音频线路。为了处理这个，iOS会自动显示一个控制器让用户选择一个输出的音频线路（使用[MPVolumeView](https://developer.apple.com/library/ios/documentation/MediaPlayer/Reference/MPVolumeView_Class/index.html#//apple_ref/occ/cl/MPVolumeView)类来让控制器显示在你的app中）。因为选择一个不同的音频线路是一个用户发起的动作，他们期望当前播放的声音不要暂停地继续播放。

`如果你需要显示一个音量滑动条，`当你使用[MPVolumeView](https://developer.apple.com/library/ios/documentation/MediaPlayer/Reference/MPVolumeView_Class/index.html#//apple_ref/occ/cl/MPVolumeView)类时确保使用系统提供的音量滑动条。注意当当前使用的声音输出设备不支持音量控制时，音量滑动条会被合适的设备名替换。

`如果你的app只产生对功能不是必须的UI音效，那么就使用系统声音服务。`系统声音服务时一个产生警告框、UI音效和震动的iOS技术；它不适用于任何其他目的。当你使用系统声音服务来产生声音时，你不能影响你的声音与设备上的声音的交互方式，以及它被设备配置打断和更改时的响应。查看[Audio UI Sounds (SysSound)](https://developer.apple.com/library/ios/samplecode/SysSound/Introduction/Intro.html#//apple_ref/doc/uid/DTS40008018)获取示范使用这个技术的简单工程。

`如果声音在你的app中扮演了很重要的角色，使用音频会话服务或者AVAudioSession类。`这些编程接口不产生声音；它们帮助你表达你的声音和设备上的声音应有的交互方式以及对设备配置打断和更改的响应。

`IPHONE`
无论你使用何种技术产生声音或者定义它的行为，手机都可以中断当前运行的app。这是因为没有app应该保护人们免于收到来电。

在音频会话服务中，音频会话功能作为你的app和系统之间的一个声音媒介。其中一个最重要的方面就是类别（category），这定义了你app中声音的行为。

为了体会音频会话服务的优势以及提供用户期待的声音体验，你需要选择最能描述你app中声音行为的类别。这里是你的app是只能在前台播放声音还是也能在后台播放的情况。当你进行这个选择时遵循下面的指南：

* `基于语义选择音频会话类别，而不是它精确地一系列行为。`通过目的清晰地选择一个类别，你确保你的app按照用户期待的方式来行为。此外，这给了你的app最好的机会来在未来一系列的行为改善时表现得合适。
* `在很少的情况下，添加一个恰当的音频会话来修改一个类别的标准行为。`一个类别的标准行为代表了用户最期待的内容，所以在你改变行为前要仔细地考虑。比如说，你可能会恰当地添加紧急降低来确保你的声音比所有其他的声音都低（尤其是来电声音），如果这是用户期望你的app做的话。（查看[Fine-Tuning a Category](https://developer.apple.com/library/ios/documentation/Audio/Conceptual/AudioSessionProgrammingGuide/AudioSessionBasics/AudioSessionBasics.html#//apple_ref/doc/uid/TP40007875-CH3-SW8)来学习更多关于音频会话属性的内容。）
* `考虑基于予你当前设备的声音环境来选择类别。`这在某些情况下，比如，用户可以在听其他声音而不是你的声道时使用你的app，就会有意义。如果你这样做，确保避免在你的app启动时让你的用户停止他们正在听的音乐或者进行一个声道的选择。
* `一般来说，在你的app运行时避免改变类别。`主要的改变类别的原因是你的app需要在不同的时间支持录音和播放的时候。这种情况下，在录音类别和播放类别之间按需转换会比选择播放和录音类别好。因为选择录音类别可以确保在录音中不想起提示音——比如收到短信的提示音。

表1列出了你可以使用的音频会话类别。不同的类别允许声音被静音开关（或者设备锁屏）静音、和其他声音混合或者当app在后台时播放声音。（查看[Audio Session Programming Guide](https://developer.apple.com/library/ios/documentation/Audio/Conceptual/AudioSessionProgrammingGuide/Introduction/Introduction.html#//apple_ref/doc/uid/TP40007875)获取他们在编程接口中的合适名称和实际类别。）

表1 音频会话类别和他们关联的行为

类别 | 意义 | 可静音 | 可混合 | 可后台播放
--- | --- | --- | --- | ---
独奏氛围 | 声音会加强app的功能，并且应该静音其他声音 | 是 | 否 | 否
氛围 | 声音会加强app的功能但不应该静音其他声音 | 是 | 是 | 否
播放 | 声音对app功能是必要的而且可能和其他声音混合 | 否 | 否（默认）；是（当添加和其他声音混合的性能时） | 是
录音 | 音频是用户记录的 | 否 | 否 | 是
播放和录音 | 声音代表音频的输入和输出，顺序或同时的 | 否 | 否（默认）；是（当添加和其他声音混合的性能时） | 是
音频处理 | App执行借助硬件的音频编码（不播放或录音） | 不适用 | 否 | 是

如果你选择音频处理类别并且想要在后台执行音频处理，你需要保护你的app避免在完成音频处理之前被挂起。查看Implementing Long-Running Background Tasks学习如何这样做。

这里是一些情景，可以说明如何选择一个提供用户期待的音频体验的音频会话类别。

`情景一：一个帮助人们学习一门新语言的教育类app。`你提供：
* 当用户点击特殊的控件时播放反馈音
* 当用户想要听准确发音的示例时播放单词和短语的录音。

在这个app中，声音对主要功能是必须的。人们使用这个app来听他们正在学习的语言的单词和短语，所以即使设备锁了或者切换到静音了也应该播放声音。因为用户需要清洗地听到声音，他们期待其他他们可能播放的音频静音。

为了产生用户期待这个app所有的音频体验，你应该使用播放类别。即使这个类别可能允许和其他音频混合，这个app应该使用默认行为来确保其他的音频不和用户明确选择去听的教育内容相竞争。

`情景二：一个网络电话（VoIP）app。`你提供：
* 接受音频输入的能力
* 播放音频的能力

在这个app中，声音对主要功能是必须的。人们使用这个app来与他人交流，并且经常在他们使用不同的app的时候。用户期待当他们切换静音或者锁上设备的时候也能收到电话，并且他们期待在对话期间其他音频是静音的。他们也期待当app在后台时能够持续通话。

为了产生用户期待这个app所有的音频体验，你应该使用播放和录音类别，并且你要确保你的音频会话只在你需要的时候活动，这样用户就可以在通话之间使用其他的音频。

`情景三：一个允许用户指导一个角色完成不同任务的游戏。`你提供：
* 多种游戏音效
* 一个音乐配乐

在这个app中，声音很好地加强了用户体验，但对主任务不是必要的。同样，用户希望可以静音地玩游戏或者听他们音乐库的音乐而不是游戏配乐。

最好的策略是判断用户在启动你的app的时候是否在听其他音频。不要要求用户选择是继续听其他音频还是挺你的配乐。相反，使用音频会话服务的功能[AudioSessionGetProperty](https://developer.apple.com/library/ios/documentation/AudioToolbox/Reference/AudioSessionServicesReference/index.html#//apple_ref/c/func/AudioSessionGetProperty)来询问[kAudioSessionProperty_OtherAudioIsPlaying](https://developer.apple.com/library/ios/documentation/AudioToolbox/Reference/AudioSessionServicesReference/index.html#//apple_ref/c/econst/kAudioSessionProperty_OtherAudioIsPlaying)属性的状态。给予这个询问的回答，你可以选择氛围或者独奏氛围类别（两个类别都允许用户静音玩游戏）：
* 如果用户在听其他音频，你应该假设他们倾向于继续听并且不想被强制听游戏配乐。在这种情况下，你应该选择氛围类别。
* 如果用户在启动你的app时没有在听任何其他音频，你应该选择独奏氛围类别。

`情景四：一个提供准确、实时的用户目的地的导航指令的app。`你提供：
* 对行程的每一个语音播报方向
* 少量的反馈音
* 用户继续听他们自己的音频的能力

在这个app中，无论app是否在后台，语音导航指令代表了主要任务。因此，你应该使用播放类别，允许你的音频在设备被锁、切换到静音或者在后台时播放音频。

为了允许人们在使用你的app时听其他音频，你可以添加[kAudioSessionProperty_OverrideCategoryMixWithOthers](https://developer.apple.com/library/ios/documentation/AudioToolbox/Reference/AudioSessionServicesReference/index.html#//apple_ref/c/econst/kAudioSessionProperty_OverrideCategoryMixWithOthers)属性。然而，你也希望确保用户在他们当前播放的音频之上可以听清语音指令。因此，你可以对音频会话申请[kAudioSessionProperty_OtherMixableAudioShouldDuck](https://developer.apple.com/library/ios/documentation/AudioToolbox/Reference/AudioSessionServicesReference/index.html#//apple_ref/c/econst/kAudioSessionProperty_OtherMixableAudioShouldDuck)属性来确保你的音频比其他所有正在播放的音频要响，不过iPhone的手机音频除外。这个设置允许app在后台的时候恢复其音频会话的活动，确保用户可以获取导航的实时更新。

`情景五：一个允许用户更新他们的文本和图形到网页的博客app。`你提供：
* 你简短的启动声音文件
* 伴随用户动作的多种简短音效（比如当一个提交上传时播放的声音）
* 当提交失败时的警告音

在这个app中，声音加强了用户体验，但不是必须的。主任务与音频没有关系，而且用户不需要听到任何声音来成功地使用app。在这种情景下，你应该使用系统声音服务来产生声音。这是因为app中所有声音的音频环境都遵循这个技术的预期使用目的，即产生符合用户期待的遵守设备锁屏和静音开关的方式的UI音效和警告音。

#### 管理音频中断
有时候，当前播放的音频会被其他app的音频打断。在iPhone上，比如说，一个打过来的电话会在通话期间打断当前app的音频。在多任务环境下，这种音频中断的频率会很高。

为了提供一个用户喜欢的音频体验，iOS依靠你来：
* 识别你的app可以导致的音频中断类型
* 当你的app在音频中断结束后继续时响应合理

每个app都需要识别它能够导致的音频中断类型，但不是每个app都要决定如何响应音频中断的结束。这是因为大部分类型的app应该通过回复音频来响应音频中断的结束。只有那些主要或部分播放媒体的app——和那些提供媒体播放控件的app——需要额外定义合适的响应。

概念上说，有两种类型的音频中断，基于导致中断的音频类别和用户期待app在中断结束时响应的方式：
* 可恢复中断是由用户在主要聆听体验中临时查看的音频导致的。

在可恢复中断结束后，显示媒体播放控件的app应该恢复在中断发生时进行的内容，无论是播放音频还是保持暂停。没有媒体播放控件的app应该恢复播放音频。

比如说，考虑一个用户正在iPhone上听一个音乐播放app，在音乐中间收到一个VoIP电话。用户答复这个电话，期待在他们通话的时候播放app能够静音。在通话结束后，用户期待这个播放app自动地回复播放音乐，因为音乐——而不是通话——构成了他们的主要聆听体验并且他们没有在电话到来前暂停音乐。另一方面如果用户在电话到来前暂停了音乐播放，他们会期待音乐在通话结束后保持暂停。

其他可以导致可恢复中断的app有闹钟、音频提示（比如语音提示驾驶方向）等其他中断音频。

* 不可恢复中断是由用户作为主要聆听体验的音频，比如媒体播放app的音频，造成的。

在不可恢复中断结束后，显示媒体播放控件的app不应该恢复播放音频。没有媒体播放控件的app应该恢复播放音频。

比如说，考虑用户聆听一个音乐播放app（音乐app1），而另一个不同的音乐播放app（音乐app2）打断了。作为响应，用户决定听一段时间的音乐app2。在退出音乐app2之后，用户不期望音乐app1自动恢复播放，因为他们有意让音乐app2变成他们的主要聆听体验。

下面的指南帮助你决定提供什么信息以及如何在一个音频中断结束后继续。

`识别你的app可以导致的音频中断类型。`当你的音频终止时通过在下面两种方式中的一种来停止你的音频会话。
* 如果你的app导致一个可恢复中断，伴随[AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation](https://developer.apple.com/library/ios/documentation/AVFoundation/Reference/AVAudioSession_ClassReference/index.html#//apple_ref/c/econst/AVAudioSessionSetActiveFlags_NotifyOthersOnDeactivation)标识停止你的音频会话
* 如果你的app导致一个不可恢复中断，不要伴随任何标识来停止你的音频会话

提供或不提供，这个标识允许iOS给中断的app能力来自动恢复播放它们的音频。

决定当一个音频中断时你是否应该恢复音频。你基于这个决定来提供你app的音频音频用户体验。
* 如果你的app显示人们用来播放或暂停音频的媒体播放控件，你需要在一个音频中断结束时检查[AVAudioSessionInterruptionFlags_ShouldResume](https://developer.apple.com/library/ios/documentation/AVFoundation/Reference/AVAudioSession_ClassReference/index.html#//apple_ref/c/econst/AVAudioSessionInterruptionFlags_ShouldResume)标识。

如果你的app接收到应该恢复的标识，你的app应该：
* 如果你的app在中断发生的时候正在播放音频，则恢复播放
* 如果你的app在中断发生的时候没有播放音频，则不恢复播放
* 如果你的aoo不显示播放或暂停的控件，你的app应该总是在音频中断结束的时候恢复自己的播放音频，无论是否提供了应该恢复的标识。

比如说，一个播放配乐的游戏应该总是在中断结束后自动恢复播放配乐。

#### 合适的话，处理媒体远程控制事件
app可以在用户使用iOS媒体控件或者配件控件的时候接收远程控制事件，比如耳机控件。这允许你的app接收用户从你的UI以外的地方输入的信息，无论你的app当前是在前台还是后台播放音频。

app可以发送视频给支持AirPlay的硬件——比如Apple TV——并且当播放继续时过渡到后台。这种app可以接收用户通过远程控制事件输入的信息，这样用户就可以在app在后台时控制视频的播放。此外，这种类型的app也可以在后台的时候在中断结束后恢复音频会话。

尤其是，一个媒体播放app需要合适地响应媒体远程控制事件，特别是当它在后台播放音频或者视频的时候。

为了满足当你的app在后台时播放媒体相关的职责，确保遵循下述指南：

`有意义的时候限制你的app接收远程控制事件的时间。`比如说，如果你的app帮助用户阅读内容、搜索信息和聆听音频，它应该只在用户在音频环境下的时候接收远程控制事件。当用户离开音频环境后，你应该放弃接收事件的能力。如果你的app让用户在支持AirPlay的设备上播放音频或视频，它应该在媒体播放期间接收远程控制事件。遵循这些指南允许用户假设一个不同的app媒体——并且用耳机控件控制它——当他们在你app中无媒体环境的时候。

`尽可能地使用系统提供的控件来提供AirPlay支持。`当你使用[MPMoviePlayerController](https://developer.apple.com/library/ios/documentation/MediaPlayer/Reference/MPMoviePlayerController_Class/index.html#//apple_ref/occ/cl/MPMoviePlayerController)类来支持AirPlay播放时，你可以从允许用户选择当前范围内的AirPlay设备的标准控制中获益。或者你可以使用[MPVolumeView](https://developer.apple.com/library/ios/documentation/MediaPlayer/Reference/MPVolumeView_Class/index.html#//apple_ref/occ/cl/MPVolumeView)类来显示用户可以选择的支持AirPlay音频或视频的设备。用户习惯这些标准控件的表现和行为，所以他们知道如何在你的app中使用它们。

`不要重新改变事件的目的，即使事件在你的app中没有意义。`用户期待iOS媒体控件和配件控件在所有app中的功能一致。你不用处理你app不需要的事件，但你处理的事件必须产生用户期待的体验。如果你重新定义一个事件的意义，你会迷惑用户并且可能导致他们进入一个无知的状态。

### <a name="VoiceOver"/>VoiceOver
#### 旁白
VoiceOver增加对盲人、低视力和有学习挑战的用户的亲近度。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/VoiceOver/1.jpeg)

为了确保VoiceOver用户可以使用你的app，你也许需要在你的用户界面提供一些对视图和控件的描述信息。支持VoiceOver不需要你改变任何你的UI视觉设计。

当你通过完全标准的方式使用标准UI元素的时候，你就几乎不需要做额外的工作。你的UI越定制化，你就需要提供越多的定制信息使VoiceOver可以准确地描述你的app。

让你的iOS app亲近VoiceOver用户可以增加你的用户基础和帮助你进入新市场。支持VoiceOver也可以帮助你解决由不同管理部门创建的亲近指南。

### <a name="Routing"/>Routing
#### 线路选择
地图可以显示大量可供选择的到达用户目的地的线路：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Routing/1.jpeg)

地图也可以显示一个线路app的列表——包括安装在设备的app和App Store中的——当用户想要线路的额外信息的时候。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Routing/2.jpeg)

一个线路选择app会提供当前选择线路的运输选项信息。人们期望线路选择app要快速、易于使用并且——最重要的——精确。遵循这个章节的指南可以帮助你给用户他们信任的运输信息和他们喜欢的用户体验。

`IMPORTANT`  
地图给人们他们线路的驾驶和行走方向。线路选择app提供运输信息，专注于一步步的交替运输方式——比如公交车、火车、地铁、轮渡、自行车、步行、飞机等等。  
如果你的app不提供用户指定的线路的运输信息，不要标记它为线路选择app。

`提供你app承诺的功能。`当人们在运输列表看到你的app时，他们假设它可以帮助他们到达他们的目的地。但如果你的app不能提供所选线路的信息——或者它不包括它显示包括的运输类别——人们就不会给它第二次机会。准确地表述你的app的能力很必要；否则，你的app就会看起来故意误导用户。

有两种主要的方式可以给用户对你的线路选择app信心：
* 尽可能精确地定义地理区域。比如说，如果你的app帮助人们获取巴黎的公交车信息，你支持的区域应该是巴黎，不是法兰西岛，也不是法国。
* 明确你支持的运输方式。比如说，如果你专门处理地铁信息，不要暗示你提供铁路运输方式的信息。

`NOTE`  
虽然准确地报告你支持的区域意味着你的app在运输列表中出现的少一些，但这样做会让用户更信任一些。

`精简UI来易于使用。`易于使用对线路选择app很重要，因为人们通常在有困难的时候使用它们——比如在明亮的阳光下或者火车昏暗的室内、颠簸的骑行中以及当他们很匆忙的时候。确保你的文本在任何光照下都易于阅读并且即使在不平滑的骑行下按钮也易于精准地点击。

`专注于线路。`虽然补充的信息会有帮助，你的app应该专注于给用户一步步的指导让他们可以跟随去到他们的目的地。特别是，你希望用户知道他们当前在哪一步以及如何去到下一步。你可以提供额外的信息——比如时间表和系统地图——但不要让这个信息比运输信息更显著。

`为线路的每一步提供信息。`人们不应该感到被你的app所抛弃。但即使你准确地报告了你支持的区域，你不能假设用户已经在线路的第一个运输点，或者最后一个运输点在他们目的地的相同位置。为了处理这个情况，首先计算线路的开始和结束的距离。如果距离足够短，提供从用户当前位置到第一个运输点和从最后一个运输点到用户最终目的地的步行方向。如果步行不是一个好的选择，尝试描述用户的其他选项。如果必要的话，你可以给用户一个方式来打开地图获取这部分线路的步行或驾驶方向。

`当用户从地图过渡到你的app，不要要求他们重新提供信息。`如果用户是从地图来的，你已经知道了他们感兴趣的开始和结束线路，所以你可以在你app打开的时候尽可能快地显示合适的运输信息。如果用户从主屏幕启动你的app，提供一个简单的方式让他们输入线路细节。

`用图表和文字来展现运输信息。`地图视图可以帮助人们在一个宏观的、物理的环境下查看他们完整的线路；一个步骤列表可以帮助人们关注他们到达目的地必须执行的动作。最好你支持这两种任务并且让用户可以很简单地切换。

`NOTE`  
无论何种形式，始终显示同样的关于用户线路的运输信息最重要。比如说，如果一个线路有五个步骤组成，地图和列表视图都必须描述同样的五个步骤。

当你的app被从运输列表中选择后，启动来在地图视图显示完整的线路会比较好——包括到运输点和从运输点离开的步行路径。地图视图给用户一个他们旅途的多个步骤的综览，并且显示出他们的线路是如何同周边的地理区域契合的。

`用额外的信息丰富地图。`人们期待你app中的地图和他们用过的其他地图行为相似。除了让用户缩放和平移，你应该显示标注来给用户他们需要的信息。比如说，你可以显示插针来表示用户当前的位置、目的地以及路线中的中转点。确保不要只显示一个简单的插针，因为如果没有额外的文本用户很难知道它代表什么。查看[Map View](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW134)获取更多在app中使用地图视图的信息。

尽可能的，在地图视图中整合静态地图——比如一个地铁系统地图。一个好的方式是在地图视图上覆盖静态图片，这样用户就可以查看他们的线路以及他们当前的位置是如何和大的运输系统关联的。

`NOTE`  
如果你决定显示一个静态地图图片，确保使用高分辨率图片来在用户缩放时保持高的质量。

`给用户不同的方式来排序多种运输选项。`很多因素会影响人们的运输决定——比如时间、天气以及他们关心的价格——所以让对比运输选项变得简单很重要。比如说，你可以让用户通过开始和结束时间、需要步行的数量、路途中的运输点数量或者需要的交通工具的数量来进行排序。无论你在什么列表中显示多个运输选项，确保用户可以立即区分选项之间的区别。

`考虑使用推送通知来给人们关于他们线路的重要信息。`尽可能的，让人们知道运输信息何时回改变，这样他们就可以调整他们的计划。比如说，如果一辆火车延迟了或者一个公交线路临时不可获取了，人们可能会需要选择一个不同的线路到达他们的目的地。而对于包含步骤间长时间等待的线路，人们也许会喜欢被通知他们的交通工具即将发起下一班。

### <a name="Edit Menu"/>Edit Menu
#### 编辑菜单
用户可以显示一个编辑菜单来在文本视图、网页视图和图像视图执行诸如剪切、粘贴和选择的操作。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Edit%20Menu/1.jpeg)

你可以调整一些菜单的行为来在你的app中给用户给多的内容控制。比如你可以：
* 指定哪一个标准菜单命令对当前的环境合适
* 在菜单显示之前决定菜单的位置这样你就可以保护你app UI中重要的部分免于被遮挡
* 当用户双击来显示菜单时决定默认选中的对象

你不能改变菜单它自己的颜色和形状。

查看[Copy, Cut, and Paste Operations](https://developer.apple.com/library/ios/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/UsingCopy,Cut,andPasteOperations/UsingCopy,Cut,andPasteOperations.html#//apple_ref/doc/uid/TP40009542-CH11)获取如何在代码中实现这些行为的信息。

为了确保你app中的编辑菜单行为符合用户的期待，你应该：

`显示在当前环境有意义的命令。`比如说，如果没有内容被选中，菜单不应该包含复制和剪切，因为这些命令是对选中内容操作的。同样的，如果某些东西被选中了，菜单就不应该包含选择。如果你在一个自定义的视图支持编辑菜单，你要对确保菜单显示的命令适合当前的环境负责。

`调节你布局中显示的菜单。`iOS在插入光标或选择内容的上面或下面显示编辑菜单，这取决于可使用的空间，并且放置菜单指针这样用户就可以看到菜单命令是如何和内容关联的。必要的话，你可以编码在菜单显示之前决定菜单的位置这样你就可以保护你app UI中重要的部分免于被遮挡。

`支持用户可以唤起菜单的所有手势。`虽然触摸和长按手势是用户显示编辑菜单的主要方式，他们也可以在文本视图中双击一个单词来选择单词并同时显示菜单。如果你在一个自定义的视图中支持菜单，确保响应所有的手势。此外，你可以定义用户双击时默认选中的对象。

`不要在你的UI中创建一个可以在编辑菜单中获取的命令的按钮。`比如说，让用户使用编辑菜单执行复制操作比提供一个复制按钮要好，因为用户会想知道为什么在你的app中有两种方式去做同一件事情。

`如果对用户有用的话，考虑支持静态文本你的选中。`比如说，一个用户可能想复制一个图片的标题，但他们不想复制标签元素或者视图标题的label，比如账目。在文本视图中，单词的选中应该是默认的。

`不要让按钮标题可选中。`一个可选中的按钮标题会让用户很难不激活按钮的情况下显示编辑菜单。一般来说，行为类似按钮的元素不需要被选中。

`将支持撤销与重复和对复制与粘贴的支持联合起来。`人们经常在改变想法的时候期望能撤销最近的操作。因为编辑菜单在执行动作前不会请求确认，你需要给用户机会去撤销和重复这些操作。

如果你需要创建类似下方的自定义的编辑菜单元素，遵循这些指南：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Edit%20Menu/2.jpeg)

`直接在用户选中内容上方创建编辑、更改或其他动作的编辑菜单。`人们期待标准菜单条目在当前环境文本或对象的上方操作，并且最好你自定义的菜单条目也有类似的行为。

`在所有系统提供的条目后面列出自定义的条目。`不要在系统提供的条目中散布你的自定义条目。

`保持自定义菜单条目的数量合理。`你不想要过多的选项淹没你的用户。

`为你的自定义菜单条目使用简洁的名字并确保名字精确地描述了命令的功能。`一般来说，条目名应该是描述执行的动作的动词。虽然你通常应该使用一个单一的大写单词作为条目名，如果你一定要使用短语的话，使用标题风格的大写。（简短地说，标题风格的大写意味着大写每个单词，除了文章、并列连词和四个字母或以下的介词。）

### <a name="Undo and Redo"/>Undo and Redo
#### 撤销与重做
用户通过摇动设备来发起一个撤销操作，这会显示一个警告框来让他们：
* 撤销他们刚刚输入的内容
* 重新输入以前未完成的输入
* 取消撤销操作

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Undo%20and%20Redo/1.jpeg)

你可以在你的app中以一种更一般的方式来支持撤销操作，通过说明：
* 用户可以撤销或重做的动作
* 在何种情况下你的app应该将一个摇动事件看做一个撤销手势
* 支持何种程度的撤销

查看[Undo Architecture](https://developer.apple.com/library/ios/documentation/Cocoa/Conceptual/UndoArchitecture/UndoArchitecture.html#//apple_ref/doc/uid/10000010i)学习如何在代码中实现这个行为。如果你的app支持撤销与重做，遵循下面的指南来提供一个好的用户体验。

`提供简短的描述短语来精确地告知用户他们正在撤销或重做的是什么。`iOS会自动为撤销警告框的按钮标题提供“撤销”和“重做”短语（包括在短语后的一个空格），但是你需要提供一或两个词语来描述用户可以撤销或重做的动作。比如说，你可能提供词语“名字”或“地址更改”，来创建一个类似“撤销名字”或“重做地址更改”的按钮标题。（注意警告框的取消按钮不可以被更改或移除。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Undo%20and%20Redo/2.jpeg)

`不要提供太长的文本。`太长的按钮标题会被截断而且用户会很难辨识。并且因为这是一个按钮标题，使用标题风格的大写且不要添加标点符号。

`不要过载摇动手势。`即使你可以编程设置何时将一个摇动事件视为撤销操作，如果他们同时在使用摇动来执行一个不同的动作，会使用户迷惑。分析你app中用户的交互并且不要造成用户不能理解摇动手势的结果的情况。

`只在撤销和重做是你app的功能时使用系统提供的撤销和重做按钮。`记住摇动手势是用户请求撤销和重做的主要方式，并且提供两种不同的方式来执行同样的任务会变得迷惑。如果你认为提供明确的、专用的撤销和重做控件很重要，你可以将系统提供的按钮放在导航栏。（查看[Toolbar and Navigation Bar Buttons](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW33)学习更多关于这些按钮的内容。）

`清晰地将撤销和重做的功能关联到用户当前的环境，而不是早先的环境。`考虑你允许撤销和重做的环境。一般来说，用户期望他们的更改和操作可以立即生效。

### <a name="Keyboards and Input Views"/>Keyboards and Input Views
#### 键盘和输入视图
在iOS 8及以后的系统中，你可以创建一个自定义的键盘扩展让人们在大部分地方都可以使用它，而不是系统提供的键盘。查看[App Extensions](http://blog.csdn.net/cloudox_/article/details/50392075)学习更多关于管理包括键盘在内的app扩展的指南；查看[Custom Keyboard](https://developer.apple.com/library/ios/documentation/General/Conceptual/ExtensibilityPG/Keyboard.html#//apple_ref/doc/uid/TP40014214-CH16)学习如果开发自定义键盘扩展。

合适的话，你也可以在你的app中设计一个自定义的输入视图来代替系统提供的键盘。比如说，Numbers提供了多种输入视图来使输入账户、日期和其他值变得简单和高效。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Keyboards%20and%20Input%20Views/1.jpeg)

如果你提供一个自定义的输入视图，确保它的功能对用户来说是明显的。

你也可以提供一个自定义的位于键盘（或者你的自定义输入视图）上方的输入附属视图。比如说，在一些环境下，Numbers显示一个输入附属视图来帮助用户执行标准的或自定义的表格数据计算。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/iOS%20Technologies/Keyboards%20and%20Input%20Views/2.jpeg)

当人们点击你的输入视图上的自定义控件时使用标准键盘点击音来提供可以听到的反馈。查看UIDevice Class Reference中的playInputClick文档来学习如果在你的代码中添加这个声音。

`NOTE`  
标准点击音只对当前在屏幕上的自定义输入视图起作用。人们可以关闭所有的键盘点击音——包括来自你自定义输入视图的点击音——在设置 > 声音中。

## <a name="UI Elements"/>UI Elements
### <a name="Bars"/>Bars
#### 状态栏
状态栏显示了关于设备和当前环境的重要信息（像iPhone上那样）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/1.jpeg)

状态栏：
* 是透明的
* 当呈现的时候，总是出现在屏幕的顶部边缘

`API NOTE`  
你可以对整个app全局设置状态栏风格或者对单独的视图控制器设置状态栏风格。你可以查看[UIApplication Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIApplication_Class/index.html#//apple_ref/doc/uid/TP40006728)获取关于[UIStatusBarStyle](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIApplication_Class/index.html#//apple_ref/c/tdef/UIStatusBarStyle)常量的信息，查看[UIViewController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIViewController_Class/index.html#//apple_ref/doc/uid/TP40006926)获取关于[preferredStatusBarStyle](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIViewController_Class/index.html#//apple_ref/occ/instm/UIViewController/preferredStatusBarStyle)属性的信息。

`不要创建自定义的状态栏。`用户依赖一致的系统提供的状态栏。即使你可能在你的app中隐藏状态栏，在它的位置创建自定义的UI也是不合适的。

`防止滚动内容在状态栏显示。`当用户滚动时，你不想他们在状态栏区域看到一个app内容和状态栏元素混淆的内容。为了给用户一种宽敞的印象并保持最大的可读性，确保状态栏有一个下方模糊的内容组成的背景。这里是一些保持滚动内容不显示在状态栏的方式：
* 使用导航控制器来显示内容。导航控制器自动显示一个状态栏背景并且确保它的内容视图不会在状态栏的后面显示。（查看[Navigation Controllers](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/NavigationControllers.html#//apple_ref/doc/uid/TP40011313-CH2)学习更多关于导航控制器的内容。）
* 创建一个不干扰的自定义图片——例如渐变的——并且在状态栏后面显示它。为了确保图片保持在状态栏后面，你可以使用一个视图控制器来保持图片在滚动视图的上方，或者使用一个滚动视图来保持它置顶。
* 定位内容从而避免出现在状态栏区域（也就是说，由app的[statusBarFrame](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIApplication_Class/index.html#//apple_ref/occ/instp/UIApplication/statusBarFrame)属性定义区域）。如果你这样做，你应该使用窗口的背景色来在状态栏后方提供一个实心的颜色。

`不要在状态栏后面放置有干扰性的内容。`尤其是，你不会想暗示用户点击状态栏来连接你app的内容或操作你app的控件。

`永久地隐藏状态栏之前要三思。`因为状态栏是透明的，通常不需要隐藏它。长久地隐藏状态栏意味着用户必须切换出你的app来查看时间或者确认他们是否连上了WiFi。

`考虑隐藏状态栏——和所有其他app的UI——当用户正在观看全屏视频时。`如果你隐藏状态栏，确保让人们能通过一个简单的触摸回复它（和合适的被隐藏的appUI）。除非你有不得已的愿意去做，否则不要定义一个自定义的手势来重新显示状态栏，因为用户不太可能发现它和记住它。

`选择和你的app协调的状态栏内容色。`默认的外观显示深色的内容，这在浅色的app内容上方会看上去很好。而浅色状态栏内容会在深色app内容上方看上去很好。

`合适的话，显示网络活动指示器。`网络活动指示器会在状态栏显示来告诉用户漫长的网络连接正在发生。查看[Network Activity Indicator](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW44)来学习如何在你的代码中实现这个指示器。

#### 导航栏
导航栏可以给信息层级导航，并且可以选择管理屏幕内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/2.jpeg)

导航栏：
* 是透明的
* 一般显示在app屏幕的顶部，状态栏的下方。在水平方向、常规的环境下，导航栏也可以通过一个不贯穿屏幕的视图来显示，比如一个分裂视图控制器的一个面板。
* 可以在再键盘出现时、用户做出一个手势时或者当一个包含视图控制器过渡到一个垂直方向的紧致环境时隐藏
* 可以上色。（使用[tintColor](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/occ/instp/UIBarButtonItem/tintColor)给导航栏按钮上色；使用[barTintColor](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UINavigationBar_Class/index.html#//apple_ref/occ/instp/UINavigationBar/barTintColor)给导航栏背景上色。）

`API NOTE`  
导航栏被包含在导航控制器中，是一个用来管理一系列有层次的自定义视图的显示的规划性的对象。查看[Navigation Controllers](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/NavigationControllers.html#//apple_ref/doc/uid/TP40011313-CH2)、[UINavigationController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UINavigationController_Class/index.html#//apple_ref/doc/uid/TP40006934)和[UINavigationBar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UINavigationBar_Class/index.html#//apple_ref/doc/uid/TP40006887)学习更多关于在你的代码中定义导航栏的内容。

使用导航栏来导航不同的视图，并且——合适的话——提供一个控件来管理一个视图中的元素。如果你需要提供大量的控件并且不需要导航，考虑使用工具栏来代替（查看[Toolbar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW4)来学习更多）。

当用户去往导航层级的新一级时，有两件事情会发生：
* 合适的话，导航栏标题应该改成新一级的标题。
* 在导航栏的左边应该有一个返回按钮；如果有价值的话返回按钮的标题可以使上一级的标题。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/3.jpeg)

`有价值的时候，使用当前视图的标题作为导航栏的标题。`如果给导航栏写标题看起来多余，你可以让它空着。比如说，便签没有给当前的笔记上标题，因为第一行的内容就提供了用户需要的所有内容。

`考虑放置一些分隔控件在app顶层的导航栏中。`如果这样做可以平缓你的信息层级、让用户更加容易找到他们寻找的内容，那就尤为有用。如果你在导航栏使用了分隔控件，确保选择准确的返回按钮标题。（查看[Segmented Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW4)获取使用指南。）

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/4.jpeg)

`必要的话，使用提示阐述在当前屏幕用户可以做什么。`提示是一个出现在靠近导航栏顶部的简短的句子。比如说，股票使用了一个提示来确保用户理解如何找到他们想要的信息。  
如果你需要使用提示，写一个简明的、单行的以及有合适的结尾标点符合的句子。

`避免使导航栏中的控件太过拥挤，即使看起来有足够的空间。`一般来说，一个导航栏只应该包含当前视图的标题、返回按钮和一个管理视图内容的按钮。如果你在导航栏使用了分隔控件，导航栏就不该显示标题，并且除了分隔控件以外不该再包含任何其他控件。

`确保文本标题的按钮之间有足够的空间。`如果在导航栏的多个左按钮或右按钮之间没有足够的空间，文本标题会显示到一起去，让用户难以区分他们。如果你的导航栏中的按钮标题看起来太紧凑，使用`UIBarButtonSystemItemFixedSpace`来在它们之间添加合适的空间。（查看[UIBarButtonItem Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/doc/uid/TP40007519)学习更多关于常量的内容。）

`尽可能地确保自定义的导航栏和你app协调一致。`比如说，不要将不透明的导航栏和半透明的工具栏组合起来。同样，最好不要改变同一个方向不同界面导航栏的图像、颜色或透明度。

`确保自定义的返回按钮的外观和行为和系统的返回按钮一致。`用户知道标准的返回按钮允许他们在层级信息中回顾他们的步骤。如果你决定用自定义的图片代替系统提供的V字图，确保也提供一个自定义的掩模图。iOS使用掩模图来让按钮标题在过渡的时候从V图出现。

`IMPORTANT`  
不要创建多节返回按钮。返回按钮总是会将用户待到当前界面的父界面。如果你觉得不提供显示痕迹的多节返回按钮用户可能迷失，这往往意味着你应该简化信息层级。

`当用户想要专注于内容时考虑隐藏导航栏。`如果你这样做，确保让用户通过简单的手势回复导航栏，比如一个点击。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/5.jpeg)

#### 工具栏
工具栏包含了执行与屏幕视图中的对象相关的操作的控件。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/6.jpeg)

一个工具栏：
* 是半透明的
* 在iPhone上永远出现在屏幕视图的底部边缘。在iPad上也可以出现在屏幕视图的顶部边缘。
* 可以在键盘出现时、用户做一个手势时或者抱哈你的视图控制器过渡成水平紧凑环境时隐藏。

`API NOTE`  
工具栏一般包含在导航控制器（管理一系列层级的自定义视图显示的对象）内。查看[Displaying a Navigation Toolbar](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/NavigationControllers.html#//apple_ref/doc/uid/TP40011313-CH2-SW4)和[UIToolbar Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIToolbar_Class/index.html#//apple_ref/doc/uid/TP40006927)来学习更多关于在你的代码中定义工具栏的内容。

使用工具栏来提供一系列用户可以在当前环境执行的动作。

`包括在当前环境有意义的用的最多的命令。`尽可能地不要使用工具栏提供只偶尔用到的命令。

`考虑使用分栏控件（Segmented Control）来提供到当前环境不同构面或模式连接。`在工具栏使用分栏控件来显示app层级的任务或模式不是好主意，因为工具栏是特殊对应当前屏幕视图的。如果你需要给用户到你app中基本任务、视图或模式的链接，使用标签栏（Tab Bar）来代替。查看[Segmented Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW27)来学习关于分栏控件的内容；查看[Tab Bar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW52)来学习关于标签栏的内容。

`如果你需要在工具栏放置超过三个元素的话，使用图标。`因为文本标题的按钮一般使用比图片更多的空间，会很难让这些标题不挤到一起去。

`确保文本标题的按钮之间有足够的空间。`如果在工具栏的两个或更多按钮之间没有足够的空间，文本标题会挤到一起去并且用户会很难区分它们。如果按钮标题在你的工具栏中看起来太紧凑，使用`UIBarButtonSystemItemFixedSpace`来增加它们之间合适的空间。（查看[UIBarButtonItem Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/doc/uid/TP40007519)学习更多关于这个常量的内容。）

#### 工具栏和导航栏按钮
iOS提供了很多使用在内置app中的标准工具栏和导航栏按钮。查看[Bar Button Icons](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/BarIcons.html#//apple_ref/doc/uid/TP40006556-CH21-SW1)学习如何设计自定义的图标。工具栏和导航栏中的元素可以使用[tintColor](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/occ/instp/UIBarButtonItem/tintColor)属性来上色。

在表41-1中找到符号名称对应的按钮描述，在[UIBarButtonItem Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/doc/uid/TP40007519)中查看[UIBarButtonSystemItem](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/c/tdef/UIBarButtonSystemItem)的文档。

`IMPORTANT`  
对于所有标准按钮和图标，基于其意义而不是外观来使用按钮是必要的。这会帮助你的app的UI即使在某个意义的按钮改变了其外观时依然有意义。

表41-1 工具栏和导航栏可使用的标准按钮  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/7.jpeg)

除了表41-1显示的按钮之外，你也可以使用系统提供的编辑、取消、保存、完成、重做和撤销按钮来在你的app中支持编辑或其他类型的内容操作。这每个按钮的外观都由其文本标题提供。查看[UIBarButtonItem Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/doc/uid/TP40007519)中查看[UIBarButtonSystemItem](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/c/tdef/UIBarButtonSystemItem)的文档来找到这些按钮的符号名称。

最后，你也可以在工具栏中使用系统提供的信息按钮：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/8.jpeg)

#### 标签栏
标签栏让人们可以在一个app不同的子任务、视图或模式之间切换。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/9.jpeg)

`API NOTE`  
标签栏包含在标签栏控制器（管理一系列自定义视图的显示）内。查看[Tab Bar Controllers](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/TabBarControllers.html#//apple_ref/doc/uid/TP40011313-CH3)和[UITabBar](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITabBar_Class/index.html#//apple_ref/occ/cl/UITabBar)来学习更多关于在你的代码中定义标签栏的内容。

一个标签栏：
* 是半透明的
* 总是出现在屏幕的底部边缘
* 在垂直紧凑环境下一次最多显示五个标签（如果有更多的标签，标签栏会显示其中四个，并添加一个“更多”标签，来在一个列表中显示其余的标签）
* 在所有方向保持同样的高度
* 可以在标签上显示一个标记来传达app特有的信息（标记是一个红色的椭圆包含白色的文本或数字或感叹号）

使用标签栏给用户到同一个数据的不同构面或与app总功能有关的不同子任务的链接。

`一般来说，使用标签栏来管理app层面的信息。`标签栏很适合用在app的主视图中，因为这是一个很好方式来减少你的信息层级以及提供同时到不同的对等层次的信息类别或模式的链接。

`不要使用标签栏给用户操作当前屏幕的元素或app模式的控件。`如果你需要提供控件，包括显示模态视图的控件，请使用工具栏（查看Toolbar获取使用指南）。

`不要在标签功能不可用的时候移除标签。`如果你在某些情况下移除标签而其他情况不移除，回导致你的appUI不稳定和不可预知。最好的解决方案是确保所有的标签是可选的，但要解释为什么一个标签的内容不可获取。比如说，如果用户在iOS设备内没有任何歌曲，音乐app的歌曲标签会显示一个界面解释如何下载歌曲。

`在垂直常规环境下，你可能会在弹出视图或分隔视图的第二界面使用一个标签栏。`如果标签会切换或过滤那个视图的内容则这样做。然而，在弹出界面和分隔界面使用分栏控件往往会更好，因为分栏控件的外观与这些UI元素的外观整合的更好。（查看[Segmented Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW27)来获取更多使用分栏控件的信息。）

`避免太多标签栏导致拥挤。`在标签栏放置太多标签会人们很难点击到他们想要的那个。而且随着你每多显示一个标签，你都增加了你app的复杂度。

`在垂直常规环境下，避免创建一个“更多”标签。`在垂直常规环境下运行的app，屏幕专门显示一个额外的标签列表是一种可怜的空间使用。

`尽可能的，在每个方向都显示同样的标签。`最好能通过在各个方向提供同样的标签来给用户一种视觉统一的感觉。在垂直常规环境下，你可能需要居中显示在垂直紧凑环境下同样的标签。

#### 标签栏图标
iOS提供了如表41-2描述的在标签栏中使用的标准的图标。查看[Bar Button Icons](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/BarIcons.html#//apple_ref/doc/uid/TP40006556-CH21-SW1)学习如何设计自定义的标签栏图标。标签栏图标可以通过[tintColor](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIView_Class/index.html#//apple_ref/occ/instp/UIView/tintColor)属性上色。

在[UIBarButtonItem Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/doc/uid/TP40007519)中查看[UIBarButtonSystemItem](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIBarButtonItem_Class/index.html#//apple_ref/c/tdef/UIBarButtonSystemItem)的文档找到符号名称对应的按钮描述。

`IMPORTANT`  
对于所有标准按钮和图标，基于其意义而不是外观来使用按钮是必要的。这会帮助你的app的UI即使在某个意义的按钮改变了其外观时依然有意义。

表41-2 标签栏可使用的标准按钮  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/10.jpeg)

#### 搜索栏
搜索栏接收用户输入用于搜索的文本（如下，带有占位文本）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/11.jpeg)

`API NOTE`  
查看[UISearchBar](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISearchBar_Class/index.html#//apple_ref/occ/cl/UISearchBar)学习如何在你的代码中定义搜索栏。查看[UISearchDisplayController](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISearchDisplayController_Class/index.html#//apple_ref/occ/cl/UISearchDisplayController)学习更多关于显示搜索栏的内容。

搜索栏可以显示一些可选的元素，例如：
* 占位文本。这个文本可能陈述了控件的功能（比如上面显示的“搜索”）或提醒用户他们在何种环境搜索（比如“Goodle”）。
* 书签按钮。这个按钮可以提供一个访问用户想要方便再次找到的信息的捷径。比如说，地图搜索模式的书签按钮可以标记位置、最近的搜索和接触。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/12.jpeg)

书签按钮只在搜索栏中没有用户提供的或非占位符文本时显示。当搜索栏包含这些文本时，清除按钮会出现，这样用户就可以清除文本。

* 清除按钮。大多数搜索栏包含清除按钮来让用户通过一次点击清除搜索栏的内容。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/13.jpeg)

当搜索栏包含非占位符文本时，清除按钮就会出现，这样用户就可以清除文本。如果搜索栏没有用户提供的或非占位符文本，清除按钮就要隐藏。

* 结果列表图标。这个图标暗示了搜索结果的存在。当用户点击结果列表图标时，app可以显示他们最近搜索的结果。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/14.jpeg)

* 一个提示。一个描述性的标题，称为提示，可以被放置在搜索栏上方。提示是一个简短的、完整的句子，提供搜索栏的介绍或者app独特的环境。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/15.jpeg)

使用搜索栏来在你的app中提供搜索。不用使用输入框来提供搜索，因为它没有用户期待的标准搜索栏表现。

在iOS 8及以后的系统中，使用[UISearchController](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISearchController/index.html#//apple_ref/occ/cl/UISearchController)来方便地在导航栏中放置搜索栏。注意当搜索控制器的视图控制器被包含在一个导航控制器中时——像邮件中一样——当用户发起搜索时搜索栏会自动过渡成导航栏。

`选择会在你的app中补充搜索的重要性的搜索栏风格。`如果搜索时你app的主要功能，你可能会想用突出的风格；如果用户不经常需要搜索，你可能会想用最小的风格。

突出的搜索栏风格（邮件中显示的）：  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/16.jpeg)

最小的搜索栏风格（音乐中显示的）：  
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/17.jpeg)

#### 范围栏
范围栏——只在和搜索栏结合时可用——帮助用户定义搜索的范围。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Bars/18.jpeg)

`API NOTE`  
查看[UISearchBar](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISearchBar_Class/index.html#//apple_ref/occ/cl/UISearchBar)学习更多关于在你的代码中定义搜索栏和范围栏的内容。

当搜索栏出现时，范围栏可以显示在附近的位置。范围栏采用你给搜索栏定义的同样的外观。

当用户想要搜索有清晰的定义或典型的分类的内容时显示范围栏会很有用。不过，更好的是增强搜索结果这样用户就不需要自己定义他们的搜索范围了。

### <a name="Content Views"/>Content Views
#### 活动
活动表示系统提供的或自定义的任务——通过一个活动视图控制器来实现——其可以和当前的内容互动。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/1.jpeg)

`API NOTE`  
查看[UIActivity Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIActivity_Class/index.html#//apple_ref/doc/uid/TP40011974)学习更多关于在你的代码中定义活动的内容；查看[Activity View Controller](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW121)学习如何整合活动视图控制器到你的app中。
操作和分享扩展也会在活动视图控制器中显示。查看[Share and Action Extensions](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/AppExtensions.html#//apple_ref/doc/uid/TP40006556-CH67-SW3)学习更多关于这些扩展的内容。

一个活动：
* 是一个自定义的展现当用户在app中的时候app可以执行的任务的对象
* 由看起来像栏目按钮图标的图标代表的

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/2.jpeg)

用户通过在活动视图控制器中点击活动图标来初始化活动。作为回应，无论活动时可以立即执行，还是比较复杂，都会在执行任务之前反馈更多信息。

`创建一个精简的模板图片来表示你的任务。`精简的图片是iOS用来作为创建用户看到的最终图标的覆盖图的。为了创建在最终图标中看起来不错的模板图片，要遵循下面的指南：
* 使用合适透明度的黑色或白色图片。
* 不要包含阴影。
* 使用反锯齿。

活动模板图片应该在70*70pixels（高分辨率）的区域中居中。

`创建简洁地描述你的任务的活动标题。`标题会在活动视图控制器中显示在活动图标的下方。短标题是最好的，因为它在屏幕上看起来更好而且易于本地化。当标题太长时，iOS首先会收缩文本，然后——如果标题依然太长的话——截断它。一般来说，不要在活动标题中包含你的公司或产品的名字。

#### 活动视图控制器
活动视图控制器显示一个临时的视图来列出特定内容可操作的系统提供的或自定义的任务。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/3.jpeg)

`API NOTE`  
查看[UIActivityViewController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIActivityViewController_Class/index.html#//apple_ref/doc/uid/TP40011976)学习更多关于在你的代码中定义活动视图控制器的内容；查看[Activity](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW122)学习如何设计一个提供了自定义任务的活动。

一个活动视图控制器：
* 显示一个可配置的用户可以对特定内容执行的任务列表
* 可以在表单或弹层内显示，取决于环境

使用活动视图控制器给人们一个在某些方式下可以对内容执行的任务清单。这些任务可以是系统提供的——比如复制、Twitter和打印——或者是自定义的。一个常见的使用活动视图控制器的方式是允许用户发送选中的内容到社交媒体账号。

`不要创建一个显示活动视图控制器的自定义按钮。`人们习惯于在点击动作按钮时获取系统提供的任务。你会想要得益于这个被学会的行为并且避免提供一个做相同事情的替换的方式来使用户疑惑。

`确保清单中的任务是适用于当前的环境的。`你可以通过排除系统提供的任务或包含自定义的任务来改变活动视图控制器的任务清单。比如说，为了防止用户打印图片，你可以从活动视图控制器中排除打印活动。

`NOTE`  
你不能改变活动视图控制器中系统提供的任务的顺序。还有，所有的系统提供的任务都显示在自定义的任务上方。

#### 集合视图
集合视图管理有序的条目集合并且在自定义的布局中显示它们。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/4.jpeg)

`API NOTE`  
查看[Collection View Programming Guide for iOS](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/CollectionViewPGforIOS/Introduction/Introduction.html#//apple_ref/doc/uid/TP40012334)来学习更多关于在你的代码中定义集合视图的内容。

一个集合视图：
* 可以包含一些可选的视图来视觉上区分条目的子集合或者提供装饰性的内容，比如自定义背景
* 支持布局间自定义的过渡动画（集合视图默认提供用户插入、移动或删除条目的动画）
* 支持额外的手势识别来执行自定义的动作。集合视图默认识别点击（选中条目）和长按（编辑条目）。

使用集合视图给用户一个查看和操作一个集合的条目而不需要在列表中显示出来的方式。因为集合视图不强制使用严格的线性布局，所以它可以很好的显示不同大小的条目。

集合视图支持广泛的定制化，所以它可以有效地避免你创建激进的新设计带来的困惑。你会想要集合视图对用户的任务有增益；而不会想要集合视图变成用户体验的焦点。下面的指南可以帮助你创建人们期待的集合视图。

`不要在使用列表视图更好时使用集合视图。`有时候用列表展现更利于人们查看和理解信息。比如说，文本信息在滚动列表中会更利于人们简单和有效地查看与交互。

`让人们选中条目变得简单。`如果在你的集合视图中人们很难点中条目，他们就不太可能享受使用你的app。对于所有用户可能想要点击的UI对象，确保集合视图中每个条目的最小目标区域为44*44 points。

`如果你作出了动态的布局改变要使用警告。`集合视图允许你在用户查看和交互条目的时候改变它们的布局。如果你决定动态地调整集合视图的布局，确保更改是有意义的且易于用户跟踪。没有明显原因的改变集合视图的布局会给人们一种你的app不可预知且难以使用的印象。而且如果在动态改变布局时当前的焦点或环境丢失了，用户会觉得他们失去了对你app的控制。

#### 容器视图控制器
容器视图控制器管理和展示它的子视图集合——或者子控制器集合——以一种自定义的方式。系统定义的容器视图控制器的例子有标签栏视图控制器、导航栏视图控制器和分栏视图控制器（查看[Tab Bar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW52)、[Navigation Bar](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Bars.html#//apple_ref/doc/uid/TP40006556-CH12-SW3)和[Split View Controller](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW51)来学习更多关于这些元素的内容）。

`API NOTE`  
查看[UIViewController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIViewController_Class/index.html#//apple_ref/doc/uid/TP40006926)学习关于在你的代码中定义自定义的容器视图控制器的内容。

容器视图控制器没有预定义的外观和行为。

使用容器视图控制器通过自定义的方式来导航展示内容。

`询问自己一个自定义的容器视图控制器是否是真的必须的。`用户习惯于标准容器视图控制器的外观和行为，比如分栏视图控制器和标签栏视图控制器。你需要确保你自定义的容器视图的潜在优势大于用户可能发现不了或立即知道它如何工作的事实。

`确保你的自定义容器视图控制器在各个方向都可以工作。`设计在垂直和水平方向都能给用户一致的体验的容器视图控制器很重要。

`一般来说，避免绚丽的视图过渡。`当你使用故事版设计自定义的视图控制器时，定义自定义的视图间过渡动画很容易。但在大部分情况下，绚丽的视图过渡会将人们从他们的任务转移过来并且经常会降低你app的显示美感。

#### 图片视图
图片视图显示一个图片或者一系列的动画图片。

`API NOTE`  
查看[UIImageView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIImageView_Class/index.html#//apple_ref/occ/cl/UIImageView)学习更多关于在你的代码中定义图片视图的内容。

一个图片视图：
* 没有预定义的外观并且默认情况下不允许用户交互
* 检查图片和其俯视图的属性来决定图片是否应该被拉伸、匹配大小或钉在某个特定的位置上

在iOS 7及之后的系统中，包含模板图片的图片视图会提供当前的基础色给图片。

`尽可能地确保一个图片视图内的所有图片有同样的大小并使用同样的拉伸。`如果你的图片有不同的尺寸，图片视图会分开调整它们；如果你的图片使用了不同的拉伸因子，它们可能会错误的处理。

#### 地图视图
地图视图展示地理数据并支持内置的地图app提供的大部分功能（如下图所示）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/5.png)

`API NOTE`  
查看[MapKit Framework Reference](https://developer.apple.com/library/ios/documentation/MapKit/Reference/MapKit_Framework_Reference/index.html#//apple_ref/doc/uid/TP40008210)学习更多关于在你的代码中定义地图视图的内容。

一个地图视图：
* 使用标准地图数据、卫星图或两者结合来显示地理区域
* 可以显示标记（标记简单的点）和覆盖物（描绘路径或者平面区域）
* 支持程序和用户控制的拉伸和拖动

使用地图视图来给用户一个地理区域的交互视图。如果你在开发一个路径app，就使用地图视图来显示用户的路线（查看Routing来获取更多创建路径app的信息）。

`一般来说，让用户和地图交互。`人们习惯于和内置的地图app交互，并且他们希望能和你的地图以类似的方式交互。

`以统一的方式使用标准的大头钉颜色。`地图大头钉会显示你地图中感兴趣的位置点。人们习惯于内置地图app的大头钉颜色，所以最好不要在你的app中重新定义这些颜色的意义。当你使用标准大头钉颜色时，确保以下面的方式使用它们：
* 使用红色表示目的地
* 使用绿色表示出发点
* 使用紫色表示用户指定的点

#### 页面视图控制器
页面视图控制器使用两种风格中的一种来管理多页面内容间的过渡——滚动或者翻页。这个是iOS模拟器中翻页的样子：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/6.jpeg)

`API NOTE`  
查看[Page View Controllers](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/PageViewControllers.html#//apple_ref/doc/uid/TP40011313-CH4)来学习更多关于在你的代码中定义页面视图控制器的内容。

一个页面视图控制器：
* 对滚动风格没有默认外观
 * 对于翻页风格，页面视图控制器可以添加页面间的书脊外观。
* 根据特定的风格，为页面间的过渡添加动画
 * 对于滚动风格，当前页面滚动到下一页；对于翻页风格，当前页会表现地像书或笔记本的翻页一样。

使用页面视图控制器展示用户流线型获取的（比如一个故事的文本）或自然地进入版块中的（比如日历）内容。

`必要的话，创建一种自定义的方式让用户非线性地获取内容。`页面视图控制器让用户从一个页面移动到下一页或上一页；它没有给用户提供跨页面跳转的方法。如果你想要使用页面视图控制器来显示用户可能非线性获取的内容——比如一个字典或者一本书的目录——你必须实现一种自定义的方式来让用户移动到内容的不同区域。

#### 弹出框
弹出框是当人们点击一个控件或屏幕上一个区域时显示的一个临时的界面。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/7.jpeg)

`API NOTE`  
在iOS 8及以后的系统中，你可以使用[UIPopoverPresentationController](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIPopoverPresentationController_class/index.html#//apple_ref/occ/cl/UIPopoverPresentationController)来显示一个弹出框。UIPopoverPresentationController定义了一个协议来让你调整你的弹出内容的显示风格去适应当前的显示环境。比如说，在水平常规环境下，你的内容可以在弹出框中显示；在水平紧凑环境下，你的内容可以在一个全屏的模态视图中显示。

一个弹出框：
* 是一个自包含的模态视图
* 在水平常规环境下，显示一个箭头指向它出现的点
* 有半透明的背景显示背后的模糊内容
* 可以包含大范围的对象和视图，比如：
 * 列表、图片、地图、文本、网页或自定义的视图
 * 导航栏、工具栏或标签栏
 * 与当前app视图中的对象交互的控件或对象
 * （默认情况下，弹出框中的列表视图、导航栏和工具栏使用半透明的背景来让弹出框的模糊层显出。）

在水平常规环境下，操作表单总是在弹出框中显示的。

使用弹出框来显示额外的信息或者一系列与关注的或者选中的对象有关的元素。

`NOTE`  
本指南包含显示在水平常规环境下的弹出框的UI和用户体验。如果你在全屏显示的水平紧凑环境下显示弹出框，查看Modal View来获取其他全屏模态视图的指南。

不要提供“消除弹出框”的按钮。当弹出框的显示已经不必要的时候它应该自动关闭。考虑下面的情节来确定何时弹出框是不必要的：

如果弹出框|这样做
----------|------
提供影响主视图的选项，但不实现观察者|当人们做出一个选择或当他们点击弹出框以外的任何地方时，包括显示弹出框的控件，尽快地关闭弹出框。
实现观察者|当人们点击弹出框以外的任何地方时，包括显示弹出框的控件，就关闭弹出框。在这种情况下，不要在人们做出选择时尽快地关闭弹出框，因为他们可能想要做出额外的选择或者改变当前选择的属性。
完成一个任务|当人们通过点击弹出框中的按钮，比如完成或取消，来完成或取消一个任务时关闭弹出框。在这种情况下，你可能不想在人们点击弹出框以外的地方的时候关闭弹出框，因为人们完成——或放弃——任务可能很重要。或者，当人们点击弹出框以外的地方的时候保存他们的输入，就像在点击完成时做的一样。

`一般来说，当人们点击弹出框以外的区域时保存用户的工作。`不是所有弹出框都要求明确的退出，所以人们可能错误地关闭了它。只在人们点击取消按钮时抛弃人们做的工作。

`让弹出框的按钮尽可能直接指向显示它的元素。`这样做有助于人们记住弹出框的来源以及有关的任务或对象。

`确保人们可以在看不到其背后的app内容的情况下使用弹出框。`弹出框会模糊其背后的内容，并且人们无法拖拽弹出框到别的位置。

`确保同一时间只有一个弹出框在屏幕上。`你不应该在同一时间显示超过一个弹出框（或者自定义的外观和行为类似弹出框的视图）。特别是，你不应该同时显示一个谈出啊匡从另一个中出现的串联或层级的弹出框。

`不要在弹出框的顶部显示模态视图。`除了警告框，都不应该显示在弹出框的顶部。

`可能的话，允许人们通过一次点击关闭一个弹出框并打开一个新的弹出框。`这个行为会在有多个不同的打开弹出框的栏按钮时很合适，因为这让人们避免了很多额外的点击。

`不要使用太大的弹出框。弹出框不应该占据全部的屏幕。`它应该刚好能显示它的内容并且能指向它出现的地方。弹出框的高度不是固定的，所以你可以使用它来显示一长列的清单。不过一般来说，你应该尝试避免在弹出框中滚动来完成任务。注意系统可能调整弹出框的高度和宽度来让它适应屏幕。

`在弹出框内使用标准UI控件和视图。`一般来说，弹出框使用标准控件和视图的时候会看起来更好、更易于用户理解。

`确保自定义的弹出框看起来像一个弹出框。`即使通过使用[UIPopoverBackgroundView API](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIPopoverBackgroundView_class/index.html#//apple_ref/occ/cl/UIPopoverBackgroundView)可以很容易地自定义弹出框的很多视觉部分，不要创建一个用户认识不到是弹出框的设计。如果你改变太多弹出框的外观，用户就不能依赖他们以前的经验来帮助他们理解如何在你的app中使用它。

`当弹出框依然可见时改变其尺寸要谨慎。`你可能在使用它显示同样信息的最小视图和扩展视图时想要改变弹出框的尺寸。当你调整可见的弹出框的尺寸时，使用动画来表示改动通常是个好主意，因为这不会给人们一种新弹出框代替了旧弹出框的印象。

#### 滚动视图
滚动视图帮助人们查看大于滚动视图容量的内容（下面显示的图片的高度和宽度都比包含它的滚动视图要大）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/8.jpeg)

`API NOTE`  
查看[UIScrollView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIScrollView_Class/index.html#//apple_ref/occ/cl/UIScrollView)学习更多关于在你的代码中定义滚动视图的内容。

一个滚动视图：
* 没有预定义的外观
* 当它首次出现或用户和它交互时短暂地显示滚动条
* 以一种对人们来说自然的方式响应手势的速度和方向来显示内容
 * 让用户在滚动视图中拖拽内容时，内容会跟随触摸；当用户轻击内容时，滚动视图快速地显示内容并在用户触摸屏幕或内容到达边界时停止滚动。
* 可以在分页模式操作，这时拖拽和轻击操作会显示app定义的一个内容页面

使用滚动视图让用户连接大的视图——或者大量的视图——在有限的空间内。

`恰当地支持缩放行为。`如果对你的app有意义，让用户捏或双击来放大或缩小滚动视图。当你实现缩放的时候，你还应该设置对用户任务环境下有意义的最大和最小的缩放值。比如说，让用户放大文本直到一个单词填充了屏幕并不会让用户阅读内容变得简单。

`考虑结合翻页模式的滚动视图来使用页面控件。`当你想要显示由页面、全屏或者其他组件分开的内容时，你可以使用页面控件来告诉用户有多少块是可获取的以及他们当前在查看的是哪一块。

当你使用页面控件和翻页模式的滚动视图时，在页面控件的轴线上不显示滚动条是个好主意。移除滚动条专注于页面控件并给予人们一个清晰的在内容间翻页的方式。查看[Page Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW6)来获取更多在你的app中使用翻页控件的信息。

`一般来说，一次只显示已给滚动视图。`人们经常在滚动的时候进行大幅度的手势，因此避免交互到同一个屏幕上的相邻的滚动视图就变得困难。如果你决定在一个屏幕上放置两个滚动视图，考虑让它们在不同的方向上滚动，这样一个手势就不太会滚动两个视图。比如说，iPhone纵向的股票App在垂直的滚动视图上显示股票报价，而在水平滚动视图上显示公司信息。

#### 分栏视图控制器
分栏视图控制器是一个管理两个子视图控制器的展示的全屏视图控制器。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/9.jpeg)

`API NOTE`  
分栏视图控制器的每个子视图都负责一个面板的显示管理。分栏视图控制器自己显示这些子视图控制器并管理不同方向的过渡。查看[UISplitViewController Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UISplitViewController_class/index.html#//apple_ref/doc/uid/TP40009277)和[Split View Controllers](https://developer.apple.com/library/ios/documentation/WindowsViews/Conceptual/ViewControllerCatalog/Chapters/SplitViewControllers.html#//apple_ref/doc/uid/TP40011313-CH7)来学习更多关于在你的代码中定义分栏视图控制器的内容。  
在iOS 7及更早的系统中，分啦视图控制器只可以用在iPad上。

默认情况下，一个分栏视图控制器使用当前的尺寸来决定如何安排它的子视图控制器。比如说，一个分栏视图控制器：
* 尝试在水平常规环境下并排显示两个面板
* 可以在第二面板的顶部层级显示主面板，或者可以隐藏主面板到屏幕外直到需要的时候再显示，一般来说用在水平紧致环境下

你可以通过要求分栏视图控制器在一个特定的显示环境下优先关注你特定的布局来影响面板的安排。

分栏视图控制器可以包含很大范围的对象和视图，例如：
* 列表、图片、地图、文本、网页或者自定义的视图
* 导航栏、工具栏或者标签栏

`NOTE`  
即使主面板经常称为master pane，第二面板经常称为detail pane，这个关系在代码中却并不是强制的。

使用分栏视图控制器来在主面板显示持久信息，在第二面板显示相关的详情或者从属的信息。在这种设计模式下，当人们在主面板选择一个条目后，第二面板应该显示与此条目有关的信息。（你需要在代码中实现这个事件。）

`不要创建比主面板狭窄的第二面板。`如果主面板比第二面板狭窄，分栏视图控制器就不再能充满屏幕的宽度并且整体外观时不平衡的。

`不要同时在两个面板显示导航栏。`这样做会让用户非常难识别两个面板的关系。

`一般来说，以一种持久的方式表明主面板当前选中的条目。`即使第二面板的内容可以更改，它应该总是保持与主面板选中的条目相关。这个查看的经验会帮助人们理解主面板条目和第二面板内容的关系。

`合适的话，给人们可替换的方式来获取主面板。`默认情况下，在水平紧致环境下只显示第二面板，并且你提供给用户一个按钮（一般放置在导航栏）来显示和隐藏主面板。芬兰视图控制器也支持滑动手势来执行显示/隐藏操作。除非你的app使用滑动手势来执行其他功能，否则你应该让人们通过滑动来获取主面板。

#### 表视图
表视图在一个由多行组成的滚动单列清单中显示数据。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/10.jpeg)

`API NOTE`  
查看[Table View Programming Guide for iOS](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/TableView_iPhone/AboutTableViewsiPhone/AboutTableViewsiPhone.html#//apple_ref/doc/uid/TP40007451)和[UITableView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableView_Class/index.html#//apple_ref/occ/cl/UITableView)来学习更多关于在你的代码中定义表视图的内容。

一个表视图：
* 在可以分章节或分组的行中显示数据
* 提供让用户添加或移除行、选择多个行、查看关于一行条目的更多信息或显示另一个表视图的控件

iOS定义了两种风格的表视图：

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/11.jpeg)

`简单风格。`在简单风格中，行可以被分到有标题的章节中，并且在视图的右边界可以显示一个可选的垂直索引。在章节的第一个条目之前可以显示页眉，在最后一个条目之后可以显示页脚。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/12.jpeg)

`分组风格。`在分组风格中，行是显示在分组中的，其可以有页眉和页脚。一个分组的表视图总是最少包含一个条目清单分组——每一行一个列表项——并且每个分组总是最少包含一个条目。分组表视图不包含索引。

在两种风格中，表行会在用户点击选中时简短地高亮。如果一行的选择导致导航到一个新的界面，选中的行会高亮并且伴随着新的界面滑动进来。当用户导航回前一个界面时，之前选中的行会再次简短地高亮来提醒用户之前的选择（它不会持续高亮）。

iOS包含一些可以扩展表视图功能的表视图元素。除非特别注明，这些元素只适合用在表视图中。

表视图元素|名称|意义
----------|----|----
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/13.jpeg)|勾选符号|表示行已经选中了。
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/14.jpeg)|扩展指示器|显示另一个与行有关的表
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/15.jpeg)|详情指示器按钮|在一个新视图中显示与行有关的额外的细节（查看[Popover](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ContentViews.html#//apple_ref/doc/uid/TP40006556-CH13-SW19)如何在表以外的地方使用这个元素的信息）。
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/16.jpeg)|行重排序|表示行可以拖拽到表中的另一个地方。
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/17.jpeg)|插入行|向表中添加一个新行。
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/18.jpeg)|删除按钮控件|在编辑环境下，显示和隐藏行的删除按钮。
![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/19.jpeg)|删除按钮|删除行。

除了上面列出的表特有的元素，iOS还定义了刷新控件，让用户可以刷新表的内容。查看[Refresh Control](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/Controls.html#//apple_ref/doc/uid/TP40006556-CH15-SW131)来学习更多关于在你的app中使用表的刷新控件的内容。

iOS定义了四中表单元格风格，实现了简单和分组风格下表中行的大部分常规布局。每种单元格风格都最好地适应了不同类型信息的显示。

`NOTE`  
编程上，这些风格用于表视图的单元格，这是一种告诉表如何绘制行的对象。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/20.jpeg)

`Default`（[UITableViewCellStyleDefault](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableViewCell_Class/index.html#//apple_ref/c/econst/UITableViewCellStyleDefault)）。默认单元格风格包含一个在行左边界可选的图片和跟随的左对齐标题。

默认风格适用于显示不需要通过补充信息来区分的列表条目。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/21.jpeg)

`Subtitle`（[UITableViewCellStyleSubtitle](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableViewCell_Class/index.html#//apple_ref/c/econst/UITableViewCellStyleSubtitle)）。子标题风格包含一个在行左边界可选的图片，跟随的左对齐标题和在其下方的左对齐子标题。

左对齐的文本布局让列表更加易于浏览。这种表单元格风格在列表条目看起来相似时会工作地很好，因为用户可以使用详细文本中的额外信息来区分标题文本条目。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/22.jpeg)

`Value 1`（[UITableViewCellStyleValue1](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableViewCell_Class/index.html#//apple_ref/c/econst/UITableViewCellStyleValue1)）。Value 1风格显示一个左对齐的标题和同一行中右对齐的较轻字体的子标题。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/23.jpeg)

`Value 2`（[UITableViewCellStyleValue2](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableViewCell_Class/index.html#//apple_ref/c/econst/UITableViewCellStyleValue2)）。Value 2风格以蓝色字体显示右对齐的标题，紧跟着同一行显示左对齐的黑色字体子标题。图片在这种风格中不太适合。

在Value 2的布局中，文本间清爽的垂直边缘帮助用户专注于详细文本的第一个单词。

`NOTE`  
所有四个标准表单元格风格都允许额外的表视图元素，比如勾选符号和扩展指示器。添加这些元素会减少标题和子标题可使用的单元格宽度。

清晰而有效地使用表视图来显示大量或少量的信息。比如说：
* `提供用户可以选择的选项清单。`你可以使用勾选符号来告诉用户当前列表中选中的项。
使用简单或分组表视图来显示用户点击表中一行条目时的选项清单。使用简单表视图来显示用户点击一个按钮或其他不在表的行中的UI元素时的选项清单。
* `显示层级信息。`简单表风格很适合显示层级信息。每个列表条目都可以导向另一个列表中的不同子集信息。用户通过在连续的列表中选择条目来跟踪路径。扩展指示器告诉用户点击行的任何地方都会在新列表中显示子集信息。
* 显示概念上的分组信息。两种表视图风格都允许你通过信息章节间的页眉和页脚视图来提供上下文。

你也可以使用页眉页脚视图——一种1UITableViewHeaderFooterView1实例——来在页眉或者页脚显示文本或者自定义的视图。查看[UITableViewHeaderFooterView Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITableViewHeaderFooterView_class/index.html#//apple_ref/doc/uid/TP40012241)来学习如何在你的代码中使用页眉页脚视图。

当你使用表视图时遵循下面的指南：

`当用户选择列表条目时永远要提供反馈。`用户期待当他们点击列表条目时表中的行能简短地高亮一下。在点击之后，用户期待一个新视图的出现（或者行显示一个勾选符号）来表示条目被选中了。

`如果表内容是冗长的或复杂的，不要等到所有数据都获取之后再显示。`而是立即用文本数据填成屏幕上的行然后当复杂的数据获取之后——比如图片——再显示它们。这个技术可以立马给用户有用的信息并且提高了你app的响应能力。

`在等待新数据到达时考虑显示旧数据。`即使这个技术不推荐用户那些频繁处理数据变更的app，它仍然可以帮助更多静态app立即给用户一些静态信息。当你决定这样做之前，计量数据改变的有多频繁以及有多少用户依赖于快速看到新数据。

`如果数据加载的很慢或很复杂，告诉用户处理仍在继续。`如果一个表只包含复杂数据，也许很难立即显示有用的数据。在这种情况下，避免显示空行很重要，因为空行表示你的app停止了。表应该在屏幕中间显示一个旋转的活动指示器，伴随着信息文本（比如“加载中...”）。这个行为可以使用户安心。

`合适的话，给删除按钮使用一个自定义的标题。`如果这有助于用户更好地理解你的app的工作方式，你可以创建一个标题来代替系统提供的删除标题。

`尽可能地使用简洁的文本来避免截断。`截断的单词和短语会让用户很难浏览和理解。文本截断在所有表单元格风格中都是自动的，但是根据你使用的单元格风格和截断发生的位置会造成不同的问题。

`不要将索引和显示在表右边界的表视图元素结合在一起。`显示在表右边界的表视图元素——比如扩展指示器——会干扰到索引。

`如果你想要用非标准的方式布局你的表单元格，创建自定义的单元格风格。`创建自定义的表单元格风格会比标准的要更好。查看Customizing Cells来学习如何创建你自己的单元格。

#### 文本视图
文本视图接受并显示多行文本属性。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/24.png)

`API NOTE`  
查看[UITextView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITextView_Class/index.html#//apple_ref/occ/cl/UITextView)学习更多关于在你的代码中定义文本视图的内容。

一个文本视图：
* 是一个任意高度的矩形
* 当内容大到超出其边界时支持滚动
* 支持自定义的字体、颜色和对齐方式（默认情况下，文本视图显示左对齐的系统黑色字体）
* 可以支持编辑，当用户点击文本视图内部区域时会出现一个键盘（键盘输入方法和布局取决于用户的语言设置）

`总是确保文本易于阅读。`即使你可以使用属性字符串来以有创意的方式组合多种字体、颜色和对齐方式，维持文本的可读性也是必要的。支持动态类型和使用[UIFont](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIFont_Class/index.html#//apple_ref/occ/cl/UIFont)方法`preferredFontForTextStyle`来获取显示在文本视图中的文本。查看[Text Should Always Be Legible](https://developer.apple.com/library/ios/documentation/UserExperience/Conceptual/MobileHIG/ColorImagesText.html#//apple_ref/doc/uid/TP40006556-CH58-SW3)获取支持动态类型的指南；查看[Text Styles](https://developer.apple.com/library/ios/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/CustomTextProcessing/CustomTextProcessing.html#//apple_ref/doc/uid/TP40009542-CH4-SW65)获取编程信息。

`为你期待用户输入的不同类型的内容提供不同类型的键盘。`比如说，你可能会想要让用户输入URL、PIN或者电话号码变得简单。但是要注意，你无法控制键盘的输入方法和布局，这取决于用户的语言设置。

iOS提供了很多种键盘类型，每一个都为不同类型的输入设计。查看[UIKeyboardType](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UITextInputTraits_Protocol/index.html#//apple_ref/c/tdef/UIKeyboardType)文档学习可以使用的键盘类型。阅读[Managing the Keyboard](https://developer.apple.com/library/ios/documentation/StringsTextFonts/Conceptual/TextAndWebiPhoneOS/KeyboardManagement/KeyboardManagement.html#//apple_ref/doc/uid/TP40009542-CH5)学习更多关于管理你app键盘的内容。

#### Web视图
web视图是一个可以显示丰富的HTML内容的区域（如下iPhone上邮件app中导航栏和工具栏中间所显示的）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/25.png)

`API NOTE`  
查看[UIWebView](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIWebView_Class/index.html#//apple_ref/occ/cl/UIWebView)来学习更多关于在你的代码中定义web视图的内容。

一个web视图：
* 显示web内容
* 执行一些对web内容的自动处理，比如将一个电话号码转化成拨打电话

如果你有一个网页或者web app，你可能决定使用web视图来实现一个简单的为你的网页和web app提供外皮的iOS app。如果你计划使用web视图来链接你控制的web内容，一定要阅读[Safari Web Content Guide](https://developer.apple.com/library/ios/documentation/AppleApplications/Reference/SafariWebContent/Introduction/Introduction.html#//apple_ref/doc/uid/TP40002051)。

`不要使用web视图来创建外观和行为类似小型web浏览器的app。`人们期待使用iOS上的Safari来浏览web内容，所以在你的app中复制这个宽泛的功能是不推荐的。

### <a name="Controls"/>Controls
#### 活动指示器
活动指示器显示一个任务或者进程正在进行（如下文本标签所示）。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/26.jpeg)

`API NOTE`  
查看[UIActivityIndicatorView Class Reference](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIActivityIndicatorView_Class/index.html#//apple_ref/doc/uid/TP40006830)学习如何在你的代码中定义一个活动指示器。

一个活动指示器：
* 当任务在进行时旋转而任务完成后消失
* 不允许用户交互

在工具栏或者主界面使用活动指示器来显示进程正在发生，而当其结束时不提示。

`不要使用静止的活动指示器。`用户会把静止的活动指示器当成进程陷入僵局了。

`使用活动指示器来安抚用户他们的任务或进程没有僵死。`有时候当进程快结束时简单地安抚用户比提示用户要重要。

`自定义一个活动指示器来和其所在的视图和谐一致。`合适的话，整合活动指示器的尺寸和颜色来适应其所在的背景视图。

#### 新增联系人按钮
新增联系人按钮让用户新增一个额外的联系人到文本框或其他基于文本的视图。

![](https://github.com/Cloudox/iOS-Human-Interface-Guidelines/blob/master/UI%20Elements/Content%20Views/27.jpeg)

`API NOTE`  
查看[UIButton](https://developer.apple.com/library/ios/documentation/UIKit/Reference/UIButton_Class/index.html#//apple_ref/occ/cl/UIButton)来学习如何在你的代码中定义一个新增联系人按钮。

一个新增联系人按钮：
* 显示一个用户的联系人列表
* 帮助用户添加联系人到包含新增联系人按钮的视图中

使用新增联系人按钮来给你用户一个简单的方式在不适用键盘的情况下获取联系人。比如说，用户在邮件的写信界面可以在“To”文本框点击新增联系人按钮来取代输入收信人的名字。

因为新增联系人按钮是作为输入联系人信息的替换功能的，所以在不能获取到键盘输入的界面使用这个按钮不是很合适。

#### 日期选取器
日期选取器显示一个日期和事件的组合，例如小时、分钟、日和年。




未完待续...
查看最新内容参见[我的博客](http://blog.csdn.net/column/details/cloudox-column0.html)  
[回到目录](#Catalogue)
