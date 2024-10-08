# 了解C盘结构

**C盘** 在默认的情况下你可以理解为安装与运行当前系统的磁盘分区，里面包含了系统的运行的所有文件。 

对于软件而言，其他分区可能没有，但是C盘一定是存在的，因此很多软件的默认安装位置都在C盘。也许你的部分软件也是安装在C盘的。  

:::warning
不要相信任何的`格式化C盘`的言论，尽管你的系统会保护它的系统文件不被删除，但最好你也不要去干这种事。  

在大多数情况下，删除系统盘只是一个玩笑
::: 

## 了解目录
让我们用cmd命令`dir`的方式列出C盘根目录下的内容。

它们应该存在于每一个使用过的Windows系统的C盘中。

```
2024/08/14  14:17    <DIR>          Program Files
2024/08/14  14:54    <DIR>          Program Files (x86)
2024/08/14  14:17    <DIR>          ProgramData
2024/02/02  05:58    <DIR>          Users
2024/08/14  14:20    <DIR>          Windows
```

现在，让我们来一一了解一下每一个文件夹

- `Program Files` 部分64位软件的默认安装路径，里面存放着这些软件运行所需的所有文件

- `Program Files (x86)` 与上面的文件夹的作用一样，只不过是32位软件的默认目录。

- `ProgramData` 如同意思，这个目录用于存放应用的数据，但不是所有的应用的数据都在这里，这个目录是全局的，也就是Windows下所有的用户的应用的数据都存储于此(前提是软件的数据存储目录在这)

- `Users` 如同文件夹的意思“用户”，这个文件夹用于存放用户的文件。在默认的情况下，资源管理器左侧快捷栏里的如`下载`、`文档`等都存放在此文件夹内的登陆用户名的目录下。部分软件的数据存储也在`Users\AppData`目录下

- `Windows` 这个是系统运行文件的存放路径，说简单点你的系统就在里面，这个是最重要的文件夹
