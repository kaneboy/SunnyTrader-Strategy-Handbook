# 交易策略运行模型

SunnyTrader是一个运行在Windows客户端上面的程序。它并不需要额外的服务器或其它设备作为支撑，可以运行在任何受支持的操作系统中。

每一个自定义交易策略都是一个.NET类库，在它被编译成.dll文件后，将被SunnyTrader加载并运行。交易策略与SunnyTrader运行在同一个进程中。

下图显示了SunnyTrader执行程序的文件与文件夹结构。自定义交易策略的主dll文件，需要复制到其中的**Strgetys**文件夹中\(这个文件夹的名称是一个typo\)。如果自定义交易策略还依赖其它额外的dll文件\(比如在交易策略代码中，引用了一些第三方的类库\)，那么这些依赖项dll文件需要放置到**Resources**文件夹中。

![](/assets/SunnyTraderFolders.png)

**Resources**文件夹中还有一些SunnyTrader自带的库文件。在我们撰写交易策略时，会需要引用几个SunnyTrader所提供的dll文件，它们可以在**Resources**文件夹中找到。

如果你希望运行多个SunnyTrader实例，每个实例还能有不同的配置，加载不同的交易策略，那么只需要将SunnyTrader程序复制到计算机上不同的文件夹中，然后就可以互不干扰的运行它们了。注意，一个SunnyTrader是可以加载和运行多个交易策略的，所以如果你只是需要运行多个交易策略，并不需要创建多份SunnyTrader的不同拷贝。

### SunnyTrader 最低系统需求

* Windows 7 SP1 64位 或者 Windows Server 2008 R2 SP1 64位 \(或更高版本\)
* [.NET Framework 4.6.1](https://www.microsoft.com/zh-CN/download/details.aspx?id=49982) \(或更高版本\)



