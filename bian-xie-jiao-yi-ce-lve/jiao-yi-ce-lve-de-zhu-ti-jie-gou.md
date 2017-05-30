## 使用Visual Studio开发交易策略

这篇文章将讲述使用Visual Studio 2017开发交易策略的基本步骤，包括如何部署、运行和调试交易策略。

### 新建项目

每个交易策略都被封装成一个.NET类库，并最终被编译成一个.dll文件。所以，编写一个交易策略，就是编写一个标准的.NET类库。打开Visual Studio，新建项目，选择**Visual C\#**类别中的**类库\(.NET Framework\)**。

![](/assets/CreateNewProject.png)在新建项目时，你需要注意这个项目所使用的.NET Framework版本。在新建项目窗口的上方，你可以选择这个新项目的.NET Framework版本，如下图所示。SunnyTrader交易策略所支持的最低版本是4.6.1，请确认你选择了4.6.1或者更高的版本。

![](/assets/SelectNetFrameworkVersion.png)

新项目创建之后，项目中会包含一个名为Class1.cs的默认代码文件。我们并不需要它，将它从项目中删除。

### 添加必需的引用

在Visual Studio的解决方案资源管理器的项目结构中，右击引用，选择添加引用。在

























