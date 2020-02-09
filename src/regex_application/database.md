# 数据库

正则在数据库方面也有一些应用：

* `MySQL`
  * `Sequel Pro`
* `MongoDB`
  * `Mongo Compass`

## MySQL

MySQL中通配符中的逻辑，也是基本上都是参考了正则的语法和含义：

| 与LIKE搭配的通配符语法 | 含义 | 说明 |
|-------------------- | ---- | --- |
| `%` | 0或多个字符 | 类似于正则（或Windows系统中Access）中的：星号`*` |
| `_` | 单个字符 | 类似于正则（或Windows系统中Access）中的：`?`问号 |
| `[AllowableCharList]` | 允许的字符的列表 | &nbsp; |
| `[^NotAllowableCharList]` 或 `[!NotAllowableCharList]` | 不允许的字符的列表 | &nbsp; |

详见：

[【整理】MSQL中的通配符搜索：LIKE和% – 在路上](https://www.crifan.com/mysql_wildcard_search_linke_percent)

### MySQL数据库工具：`Sequel Pro`

详见：

[【基本解决】Sequel Pro中设置通配符正则的过滤条件](https://www.crifan.com/sequal_pro_set_wildchar_regex_filter_condition/)

## MongoDB

Python中用Mongo中去搜索文件名，通过regex实现不区分大小写：

【未解决】Mongo中让搜索支持不区分大小写

根据[官网解释](https://docs.mongodb.com/v2.2/reference/operator/query/regex/#pcre-matching-engine)

`MongoDB`中的`$regex`用的是：`PCRE`=`Perl Compatible Regular Expressions`

对应语法：

[$regex — MongoDB Manual](https://docs.mongodb.com/v2.2/reference/operator/query/regex/#in-expressions)

其中也有：

* `$options`
  * `i`
  * `m`
  * `x`
  * `s`
  * 等等

和其他地方，比如Python中也很类似：

[re — Regular expression operations — Python 3.7.2 documentation](https://docs.python.org/3/library/re.html#re.S)

* `re.I` = `re.IGNORECASE`
* `re.M` = `re.MULTILINE`
* `re.S` = `re.DOTALL`
* `re.X` = `re.VERBOSE`

### MongoDB的GUI工具：Mongo Compass

类似的，MongoDB的图形化工具`Mongo Compass`，在界面中搜索内容，也支持有限的正则表达式。
