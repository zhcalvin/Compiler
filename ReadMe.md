语义分析器使用帮助
===

## 功能说明：
1. 对C语言文件进行语法分析。
2. 对文法文件进行文法分析。
3. 对C语言文件进行词法分析。

## 运行

* 打开Release文件夹下的`WindowsFormsApplication4.exe`运行。

## 使用

1. 运行后，打开文法文件`Grammar.txt`，可进行操作
    - 点击文法分析，将进行文法First，Follow，select集的求解，生成预测分析表
      - 在非终结符的列表中双击一个元素，可查看对应的预测分析表
    - 点击语法分析，开始对程序进行语法分析

2. 点击语法分析后，出现文本编辑窗口。
    - 可以直接在文本编辑区输入C语言程序或者在上方菜单选择 > 文件> 打开> 选中某一个C程序文件

3. 完成编辑区操作后，点击编辑区右下方`语法制导翻译`按钮，将出现句法分析结果。
    - 关闭该句法分析结果，回到原文本编辑窗口点击右上角三地址码书签，可看到生成的三地址码。
    - 点击词法分析结果，可看到词法分析结果。
    - 右下角是符号表，点击左侧的函数名，就可在右侧看到函数内声明的变量信息。

4. 错误分析以及定位：选择错误中某一项，即可在上方高亮显示该元素所在行的句子。

## 使用提示：

1. 本语法分析器是使用的文法为`Grammar.txt`，语义动作直接编写在Grammar中，可在文件夹下找到。
2. 测试用例见 test.c
3. 运行程序后，系统将生成预测分析表expression.txt（格式：非终结符#遇到的终结符#对应的预测分析内容）
4. 功能说明见有关PPT。

## License

Code and documentation copyright 2015 the [cherise215/Compiler](https://github.com/cherise215/Compiler/graphs/contributors) Code released under the [MIT License](https://github.com/cherise215/Compiler/blob/master/LICENSE).

