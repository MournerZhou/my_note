什么是 IPython？可能很多人已经在用，却不知道它到底是什么。 根据维基百科的解释：

IPython 是一种基于 Python 的交互式解释器，提供了强大的编辑和交互功能。  

IPython 拥有：

1.  满足你各种需求的交互式 shell
2.  火爆数据科学社区的 Jupyter 内核（供 Jupyter Notebook 使用）
3.  对交互式数据可视化和 GUI 工具的完美支持
4.  简单易用的高性能并行计算工具

![](https://pic1.zhimg.com/v2-58db72a66b558d071976a7d0e977839c_r.jpg)

IPython 中的‘I’即代表交互的意思，所以 IPython 提供了丰富的工具，能更好地与 python 进行交互。  
大家经常遇到的魔法命令，就是 IPython 的众多功能之一。  
本文梳理 IPython 的 50 个用法，供 Python 爱好者参考。

注：前面说过 IPython 提供了 jupyter 内核，所以 Jupyter Notebook 是一个基于浏览器的 IPython shell，支持 IPython 的所有功能，以下内容均在 Jupyter Notebook 环境中测试。  

常用功能：
[[#**5. tab 自动补全**]]
[[#**8. `%run`运行脚本**]]


## **1. `?`打印 IPython 简介**

在 IPython 中直接输入`?`，可以打印出 IPython 的功能介绍

![](https://pic4.zhimg.com/v2-18d121c6d114139e819d8c1bf39073db_r.jpg)

## **2. `object ?`内省功能**

在变量后面加上`?`，可以打印出该变量的详细信息。 例如图中一个列表对象，打印出该对象的类型、长度等信息。

![](https://pic1.zhimg.com/v2-b38b9a2a9e49345742c702733e4555c8_r.jpg)

## **3. `object ??`内省功能**

`??`和`?`功能相似，不过`??`还可以查看函数或模块对象的源代码。

![](https://pic1.zhimg.com/v2-31bd1e7149fa1d6c83596a2cb378d42c_r.jpg)

## **4. `history`历史命令**

在 IPython 中，执行`history`或`hist`命令能够查看历史输入。

![](https://pic2.zhimg.com/v2-a67640f3fbce02aa95904021e0135159_r.jpg)

## **5. tab 自动补全**

IPython 支持 tab 键自动补全。

![](https://pic1.zhimg.com/v2-473619bf6173fd0740f64d8b5c4260c8_r.jpg)

## **6. `! shell_command`执行 shell 命令**

shell （windows 里叫作 cmd）表示使用文本与计算机进行交互的方式，在 IPython 中，shell 命令前加上感叹号`!`（英文输入法）就可以直接执行。 如图使用 ping 检测百度网址。

![](https://pic4.zhimg.com/v2-4a14122a33147b2ecd5367b4fa7f289f_r.jpg)

## **7. 魔法命令 % 和 %% 区别**

魔法命令分为两种，一种是 line magics，另外一种 cell magics。 Line magic 是通过在前面加 %，表示 magic 只在本行有效。 Cell magic 是通过在前面加 %%，表示 magic 在整个 cell 单元有效。

## **8. `%run`运行脚本**

在 IPython 会话环境中，py 文件可以通过`%run`命令当做 Python 程序来运行，输入`%run 路径+文件名称`即可。 如图，e 盘中有一 py 脚本 test.py，在 IPython 中执行。

![](https://pic4.zhimg.com/v2-0533ce175cfcc645aa65123d35c8a903_b.jpg)

![](https://pic3.zhimg.com/v2-17bf0710361018fff0a6e7c89d07cdde_r.jpg)

## **9.`%timeit`测量代码运行时间**

IPython 使用魔法命令`%timeit`来测量单行代码的运行时间。

![](https://pic4.zhimg.com/v2-d5c66cc8a2f92289f806bcc4fd75e317_r.jpg)

## **10.`%%timeit`测量代码运行时间**

`%%timeit`用来测量整个单元格代码的运行时间.

![](https://pic1.zhimg.com/v2-6d596994eb0ab023cf0ddd1bf788e83c_r.jpg)

## **11. `%pwd`显示工作路径**

该魔法命令用来显示当前工作目录的路径。

![](https://pic4.zhimg.com/v2-8734f0501e0a01edffbdfa11d1e1689f_r.jpg)

## **12. `%matplotlib inline`显示图像**

在 notebook 中绘制图像时，使用`%matplotlib inline`命令可以将图表直接嵌入到 notebook 中，方便查看。

![](https://pic1.zhimg.com/v2-b1ee006ce3edd2bf0ad2c546035f56b8_r.jpg)

## **13. `%conda`安装第三方库**

`%conda install pkgs`命令用于在 IPython 中安装 python 第三方库。

![](https://pic1.zhimg.com/v2-bb62b9f16b5dfabc63cce540a8bf341c_r.jpg)

## **14. `%pylab`交互式计算**

`%pylab` 魔法命令可以使 numpy 和 matplotlib 中的科学计算功能生效，这些功能被称为基于向量和矩阵的高效操作，交互可视化特性。它能够让我们在控制台进行交互式计算和动态绘图。

![](https://pic1.zhimg.com/v2-6e8863ef58869ebd6470c0c016f4b6a4_r.jpg)

## **15. `%quickref`查看参考**

`%quickref`用来查看 IPython 的特定语法和魔法命令参考。

![](https://pic1.zhimg.com/v2-f70291d6d25ea33396adf92d308540b0_r.jpg)

## **16. `%ls`显示目录内容**

`%ls path`命令可以用来显示特定目录下的内容。

![](https://pic2.zhimg.com/v2-cba847bdde632071dd29b3d724e76281_r.jpg)

## **17. 通配符`*`**

使用通配符`*?`可以模糊查询方法名及属性。

![](https://pic2.zhimg.com/v2-5de4ff302366190b01be987a07144a49_r.jpg)

## **18. `%cd`修改目录**

`%cd`命令可以修改当前工作目录。

## **19. `_`打印前输出结果**

使用一个下划线 `_` 获取前一个输出结果，它是个变量，实时更新的。 使用两个下划线 `__`可以获取倒数第二个输出，使用三个下划线 `___` 获取倒数第三个输出（没有输出的命令行不计入在内，只支持前三个输出结果）。

![](https://pic4.zhimg.com/v2-b57590b536116be9fb0afb02bfe5f667_r.jpg)

![](https://pic3.zhimg.com/v2-837020b0121f511a5f05408047e46956_r.jpg)

## **20. `;`抑制输出**

在语句后面加上`;`，不显示输出结果。

![](https://pic1.zhimg.com/v2-c15d4f34156aa9006816c83989572e68_r.jpg)

## **21. `%debug`交互式调试器**

`%debug`命令支持从最新的异常跟踪的底部进入交互式调试器。 在 ipdb 调试模式下能访问所有的本地变量和整个栈回溯。使用 u 和 d 向上和向下访问栈，使用 q 退出调试器。在调试器中输入? 可以查看所有的可用命令列表。

![](https://pic2.zhimg.com/v2-384e24d454e69dbcd654efb7464b798d_r.jpg)

## **22. `%pdb`交互式调试器**

`%pdb`同样用于启动交互式调试器，不过支持对所有的异常进行调试。你需要事先启动`%pdb`命令，之后对每一个异常都会进行调试。

![](https://pic3.zhimg.com/v2-5b668aee957a96759b6a18e27846e376_r.jpg)

## **23. `%run -d`交互式调试器**

`%run -d`用于对脚本进行调试。

![](https://pic4.zhimg.com/v2-b7309cd435f14bc6ceb7f6fa96e907af_r.jpg)

![](https://pic2.zhimg.com/v2-34b06e5cc3e22623cdb76a5658f9e771_r.jpg)

## **24. `%pycat`语法高亮**

`%pycat filename`用语法高亮显示一个 python 文件（不用加. py 后缀名）。

![](https://pic3.zhimg.com/v2-bd6ef60a34291f8e4a5edc7e6f6c9b16_b.jpg)

![](https://pic4.zhimg.com/v2-ddd53ca53332f70c4dfb502a38f372b7_r.jpg)

## **25. `%env`环境变量**

`%env`命令用于显示环境变量。

![](https://pic2.zhimg.com/v2-469860eb20b205d167f0bba1e7b8fb6d_r.jpg)

## **25. `%load`加载代码**

`%load`命令用于将脚本代码加载到当前 cell。

![](https://pic4.zhimg.com/v2-8eda2c1f7bf279890fe8f4be419bdd03_b.jpg)

![](https://pic1.zhimg.com/v2-38935725741c20621ccbcc2e590bf590_r.jpg)

## **26. `%macro`定义宏**

`%macro taskname n1 n2...`用来定义宏，并给宏命名，执行指定的代码行。 执行 name 就是执行 n1 n2... 这些代码。

![](https://pic4.zhimg.com/v2-6ee4bd670fdf1afcf73559a495687007_r.jpg)

## **27. `%notebook`导出 notebook**

`%notebook path`用于导出当前 notebook 内容到指定 ipynb 文件中。

![](https://pic4.zhimg.com/v2-c72bf4f62c16ef197314b9b85331a7d3_r.jpg)

## **28. `%pdef`打印构造信息**

`%pdef`命令用来打印类、函数的构造信息。

![](https://pic2.zhimg.com/v2-9795f46f8af8f5b0b095017aa676f181_r.jpg)

## **29. `%pdoc`打印文档**

`%pdoc`命令用来打印对象的文档字符串。

![](https://pic1.zhimg.com/v2-8d7375e746edc16a56d52d9c07f1ea0c_r.jpg)

## **30. `%precision`浮点数精度**

`%precision`命令用来设置浮点数精度，可添加具体参数，无参数则默认精度。

![](https://pic4.zhimg.com/v2-ddc41de5cc71fcd937cf314de196ef73_b.jpg)

## **31. `%xdel`删除变量**

`%xdel`命令用于删除变量，并尝试清楚其在 IPython 中的对象上的一切引用。

![](https://pic3.zhimg.com/v2-889ec09994772caf55f995b5931eb35a_r.jpg)

## **32. `%who`显示变量**

`%who`命令用于显示当前所有变量，你也可以指定显示变量的类型。

![](https://pic4.zhimg.com/v2-ff0e915fece3f07bbc82e13265ffdf5f_r.jpg)

## **33. `%who`显示变量**

`%who`命令同样用于显示当前变量，但提供的信息更加丰富。

![](https://pic1.zhimg.com/v2-79bea11c5b0550768d4905753ecabe8c_r.jpg)

## **34. `%save`保存 cell**

`%save path n1 n2..`命令用于将指定 cell 代码保存到指定的 py 文件中。

![](https://pic1.zhimg.com/v2-4eec1a2b49482a628a187194a149cdf4_r.jpg)

![](https://pic3.zhimg.com/v2-4c9ec45bc1bd8fb601d932e369b3c992_b.jpg)

## **35. `%reset`重置**

`%reset -f`命令用于删除定义的所有变量，如果不指定参数`-f`，则需要确认后再重置。

![](https://pic1.zhimg.com/v2-11849bae6b0c0275b808fd56417f3e68_r.jpg)

## **36. `%rerun`执行前代码**

`%rerun`命令用于执行之前的代码，可以指定历史代码行，默认最后一行。

![](https://pic1.zhimg.com/v2-57543e2673a075ee09008619ce8c3d84_r.jpg)

## **37. `%%HTML`渲染 HTML**

`%%HTML`命令用于将单元格渲染为 HTML 输出。

![](https://pic4.zhimg.com/v2-8b1b7a86d1ea718821c995d134a4ecaf_r.jpg)

## **38. `%%javascript`运行 JavaScript**

`%%javascript`命令用于运行含有 JavaScript 代码的 cell。

![](https://pic4.zhimg.com/v2-b7592d6f27aec8fafa8ceb289e2c316b_r.jpg)

## **39. `%%latex`渲染 LaTeX**

`%%latex`命令用于将 LaTeX 语句渲染为公式，LaTeX 是一种基于ΤΕΧ的排版系统。

![](https://pic2.zhimg.com/v2-b1ded11f48eaf2d29a415157aa06f995_r.jpg)

## **40. `%%markdown`渲染 markdown**

`%%markdown`命令用于将 markdown 文本渲染为可视化输出。

![](https://pic2.zhimg.com/v2-8cf94d67e8f7785c5e964789e325b9b9_r.jpg)

## **41. `%%writefile`写入文件**

`%%writefile`命令用于将单元格内容写入到指定文件中，文件格式可为 txt、py 等。

![](https://pic2.zhimg.com/v2-4b8d216b1d1374c686f696ad07f39809_r.jpg)

![](https://pic1.zhimg.com/v2-14e131892435afaaa362cc58b2641bd0_b.jpg)

## **42. `%bookmark`保存书签**

`%bookmark`命令能够保存常用目录的别名，以便实现快速跳转，书签能够持久化保存。

![](https://pic4.zhimg.com/v2-3b4d0454de561a3b78dee3ab115003f3_b.jpg)

## **43. `%paste`粘贴代码块**

当你使用 IPython 解释器时，有件事经常让你头疼，那就是粘贴多行代码块可能会导致不可预料的错误，尤其是其中包含缩进和解释符号时。  
使用`%paste`命令能够直接执行剪切板中的 python 代码块。

![](https://pic4.zhimg.com/v2-ea05f3276ceb12516ffda3df92db38fb_r.jpg)

## **44. `%magic`获取魔法命令列表**

`%magic`用于获取所有魔法命令及其用法。

![](https://pic4.zhimg.com/v2-b612fc7d7cdedeb3bb009ac9eb47678b_r.jpg)

## **45. `In`和`Out`**

常会看到 IPython 中的`In[1]:`/`Out[1]:`形式的提示, 它们并不仅仅是好看的装饰形式，还是包含输入、输出的变量。  
In 对象是一个列表，按照顺序记录所有的命令。  
Out 对象不是一个列表，而是一个字典，它将输入数字映射到相应的输出（如果有的话）

![](https://pic2.zhimg.com/v2-18f513a5092d009b9c4cdaa0f3c73b39_r.jpg)

## **46. `%xmode`控制异常**

`%xmode`命令用于控制异常输出的模式。

![](https://pic3.zhimg.com/v2-42a4dc9e3c8062f0c75f7c9235e4e602_r.jpg)

## **47. jupyter qtconsole**

jupyter qtconsole 是 ipython 团队基于 qt 框架开发的一个 GUI 控制台。  
它具有富文本编辑功能，既能够在里面实现内嵌图片、多行编辑、语法高亮等。

![](https://pic1.zhimg.com/v2-23817ffda371468701e5b86bf3223034_r.jpg)

## **48. IPython 导航快捷键**

![](https://pic3.zhimg.com/v2-16d1e6518bd901344bacace72836e86a_b.jpg)

## **49. IPython 文本输入快捷键**

![](https://pic2.zhimg.com/v2-d90d8f48501331ab8e2c40e745485b99_b.jpg)

## **50. IPython 命令历史快捷键**

![](https://pic1.zhimg.com/v2-db16b431169d8e2031a72252d0ac9b2c_b.jpg)