# iOS-Human-Interface-Guidelines
翻译自苹果官方文档《iOS Human Interface Guidelines》

## 目录
* [UI Design Basics](#UI Design Basics)
  * [Designing for iOS](#Designing for iOS)
  * [iOS App Anatomy](#iOS App Anatomy)
  * [Adaptivity and Layout](#Adaptivity and Layout)
  * [Starting and Stopping](#Starting and Stopping)
  * [Navigation](#Navigation)
  * [Modal Contexts](#Modal Contexts)
  * [Interactivity and Feedback](#Interactivity and Feedback)

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

未完待续...
