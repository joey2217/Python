# Basic

> https://www.liaoxuefeng.com/wiki/1016959663602400

> 数字

1. 除法(/)永远返回一个浮点数。
2. 如要使用 floor 除法 并且得到整数结果（丢掉任何小数部分）,使用 // 运算符；
3. 要计算余数你可以使用 %
4. ** :幂乘方

>字符串

1. 带有 \ 的字符被当作特殊字符，你可以使用 原始字符串，方法是在第一个引号前面加上一个 r
2. 字符串可以由 + 操作符连接(粘到一起)，可以由 * 表示重复:

        >>> # 3 times 'un', followed by 'ium'
        >>> 3 * 'un' + 'ium'
        'unununium'

3. 字符串也可以被截取(检索)。类似于 C ，字符串的第一个字符索引为 0 。Python没有单独的字符类型；一个字符就是一个简单的长度为1的字符串。索引也可以是负数，这将导致从右边开始计算。
4. 除了索引，还支持 切片。索引用于获得单个字符，切片 让你获得一个子字符串:


        >>> word[0:2]  # characters from position 0 (included) to 2 (excluded)
        'Py'
        >>> word[2:5]  # characters from position 2 (included) to 5 (excluded)
        'tho'

        s[:i] + s[i:] = s

>列表
1. 列表的元素不必是同一类型
2. 列表可以被索引和切片
3. 所有的切片操作都会返回一个包含请求的元素的新列表。这意味着切片操作返回列表一个新的（浅）拷贝副本
4. 列表是 可变的，它允许修改元素
>TIPS
1. 多重赋值

        a, b = b, a+b
2.  print(b, end=',')
>函数
1. 定义函数 关键字 `def` 引入了一个函数定义
2.  默认参数值

        def ask_ok(prompt, retries=4, complaint='Yes or no, please!'):'
            pass
3. 函数可以通过 关键字参数 的形式来调用，形如 `keyword = value`
4. 可变参数列表:一个最不常用的选择是可以让函数调用可变个数的参数。这些参数被包装进一个元组。在这些可变个数的参数之前，可以有零到多个普通的参数:
>Lambda 形式

        通过 lambda 关键字，可以创建短小的匿名函数。lambda a, b: a+b。