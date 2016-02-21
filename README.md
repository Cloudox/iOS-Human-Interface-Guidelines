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


未完待续...
查看最新内容参见[我的博客](http://blog.csdn.net/column/details/cloudox-column0.html)  
[回到目录](#Catalogue)
