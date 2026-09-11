# 使用技巧
## IOC容器
 实现依赖注入(DIP的核心机制,用于管理组件生命周期、解耦服务依赖并支持模块化开发，默认支持多种容器（如Unity、DryIoc）)

 容器配置入口，继承PrismApplication

## view和viewModel

## 区域
是Shell或者父视图上预留的一块UI占位区域，是用来动态挂载/卸载不同模块的View，通过IRegionManager来管理<br/>
1、Xaml定义Region
```bash
<!-- Shell主窗口Xaml -->
<Window xmlns:prism="http://prismlibrary.com/">
    <DockPanel>
        <!-- 顶部菜单区域 -->
        <ContentControl DockPanel.Dock="Top" prism:RegionManager.RegionName="MenuRegion"/>
        <!-- 左侧导航树区域 -->
        <ContentControl DockPanel.Dock="Left" prism:RegionManager.RegionName="LeftNavRegion"/>
        <!-- 主内容区域（最常用，放业务页面） -->
        <ContentControl prism:RegionManager.RegionName="MainContentRegion"/>
        <!-- 底部状态栏 -->
        <ContentControl DockPanel.Dock="Bottom" prism:RegionManager.RegionName="StatusRegion"/>
    </DockPanel>
</Window>
```

## 模块化
1、两个重要的接口<br/> 
IContainerProvider 解析模块<br/>
IContainerRegistry 注册模块<br/> 
2、常见的问题总结<br/> 
(1)、导航找不到页面，检查模块视图名称有没有写错<br/> 
(2)、

## 消息对象(发布-订阅)

## 弹窗对象