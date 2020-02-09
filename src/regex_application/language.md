# 编程语言

如前所述，正则在很多编程语言中也有应用，以及很多都有内置的正则的库：

## `Python`的`re`

详见：

[Python中的正则表达式：re模块详解](http://book.crifan.com/books/python_regular_expression_re_intro/website)

### `BeautifulSoup`

`BeautifulSoup`中的`find`和`findAll`的`name`或`attr`参数，也支持正则

详见：

[【教程】BeautifulSoup中使用正则表达式去搜索多种可能的关键字 – 在路上](https://www.crifan.com/python_beautifulsoup_find_using_regular_expression/)

## `Perl`的`PCRE`

PERL语言中的正则的库：`pcre`

官网：[PCRE - Perl Compatible Regular Expressions](https://www.pcre.org)

## `PHP`

## `JavaScript`

最新`JS`的规范中：

[ECMAScript 2018 语言规范正式发布，改进正则表达式 - 开源中国社区](https://www.oschina.net/news/97609/ecmascript-2018-finally)

支持了一些正则的（其他语言的正则早就支持的）高级功能：

* 支持 s (dotAll) 模式
* Unicode 属性转义（Property Escape）
* 支持后行断言（Lookbehind Assertions）
* 命名捕获组（named capture group）

## js的正则的心得

### 问号要写成`\\?`而不是`\?`

详见：[【已解决】js中正则匹配问号出错：Invalid regular expression Nothing to repeat](http://www.crifan.com/js_regex_match_error_invalid_regular_expression_nothing_to_repeat)

### 括号`[]`中的`\w`要写成`\\w`才可以

详见：[【已解决】js中正则无法匹配短横线](http://www.crifan.com/js_regex_cannot_match_short_hyphen_das_char)

### js中对命名的组支持的不好

详见：[［不去解决］js中的正则如何写named group命名的组](http://www.crifan.com/js_regex_how_do_named_group)

## `C#`

## `Java`的`java.util.regex`

## `ActionScript`的`RegExp`

## `Objective-C`

## `Swift`的`NSRegularExpression`

swift中也支持正则

但不是很好用：

[［未解决］Swift中字符串的正则表达式处理：判断字符串是否符合某个类型 – 在路上](https://www.crifan.com/swift_string_regex_process_match_some_type/)

## Ruby

有个网站专门用于测试Ruby正则的网站：

[Rubular a Ruby regular expression editor](https://rubular.com/r/xfQHocREGj)
