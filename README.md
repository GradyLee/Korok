# 关于 Korok

Korok取自塞尔达传说里面的森林精灵，在我的最初计划里面这应该是一个面向组件的简单易扩展的2D游戏引擎，引擎的设计启发自：bitsquid.blogspot.com 。
在一般的游戏引擎中都会有游戏对象的概念，比如：Unity 的 GameObject，Cocos2D 的 Sprite，在 korok 里面，是没有这个概念的，它的本质是一个ECS系统，GameObject
是通过一个 id索引各种相关组件组成的，现在设计了几种组件：

1. RenderComp 渲染一个可渲染对象
2. Transform  负责坐标和场景图
3. Animator   动画控制器
3. SourceComp 负责音频

但是目前这些都没有实现，在最好的版本中，我实现各个子系统，但是在把它们组合在一个大的框架下时出现了各种问题，此时暴露出的最大问题是：理论有余，实践不足
所以在设计各个系统的时候我能够想到各种 "大概的" 架构和相关的优化技巧，但是在具体实施的时候常为一些琐碎的问题所困扰，举步维艰。所以我决定暂时停止这个项目的开发，
学习学习现有的知名引擎代码获得一些灵感和基础概念的构建方式。

代码暂寄于此，期，重头再来。