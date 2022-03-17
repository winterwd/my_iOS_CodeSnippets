# my_iOS_CodeSnippets
 Xcode 的 iOS 通用代码片段集

抄了一部分 [QMUI_iOS_CodeSnippets](https://github.com/QMUI/QMUI_iOS_CodeSnippets.git) 的，还有一些自己的

## 使用方式
Xcode 的 Code Snippets 文件存放于 `~/Library/Developer/Xcode/UserData/CodeSnippets` 目录，只要直接把 `*.codesnippets` 文件放到这个目录下（若没有则自己创建），重启 Xcode 即可生效。

为了方便更新，建议直接将 QMUI iOS CodeSnippets clone 到这个目录内（注意，不是在 CodeSnippets 里创建一个 QMUI 的目录，这里不支持子目录）：
```bash
cd ~/Library/Developer/Xcode/UserData/CodeSnippets
```
CodeSnippets 目录为空:
```bash
git clone https://github.com/winterwd/my_iOS_CodeSnippets.git ./
```
CodeSnippets 目录不为空:
```bash
git init .
git remote add origin https://github.com/winterwd/my_iOS_CodeSnippets.git
git pull origin master 
```

其中以 `QM_` 前缀开头的文件是通用的 Code Snippets，以 `QMUI_` 前缀开头的文件是专用于 `QMUI for iOS` 框架的代码片段。在下方的快捷键汇总里，QMUI 的代码片段将会以QMUI的形式标记出来。

注意，Xcode 对每一段 Code Snippet 都有规定适用的语言（Objective-C、Objective-C++、Swift、...）和作用域（如 Class 的 Interface 定义内、Class 的 Implementation 内、方法体内、...），所以测试某段 Code Snippet 不生效时请注意你当前是否处于不匹配的位置。
