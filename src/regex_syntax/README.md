# 正则语法

下面整理出正则表达式的语法规则：

此处以Python为例，参考：[Python Regular Expression's Cheat Sheet](http://www.pyregex.com)，正则表达式的基本语法如下：

## 正则表达式语法

文字版：

* **Special Characters**
  * `\` escape special characters
    * common char need escaple:
      * `\`
      * `[`
      * `]`
      * `(`
      * `)`
      * `{`
      * `}`
      * `.`
      * `*`
      * `+`
      * `?`
      * `^`
      * `$`
      * `|`
  * `.` matches any character
  * `^` matches beginning of string
  * `$` matches end of string
  * `[5b-d]` matches any chars '5', 'b', 'c' or 'd'
  * `[^a-c6]` matches any char except 'a', 'b', 'c' or '6'
  * `R|S` matches either regex R or regex S
  * `()` creates a capture group and indicates precedence
* **Quantifiers**
  * `*` 0 or more (append ? for non-greedy)
  * `+` 1 or more (append ? for non-greedy)
  * `?` 0 or 1 (append ? for non-greedy)
  * `{m}` exactly mm occurrences
  * `{m, n}` from m to n. m defaults to 0, n to infinity
  * `{m, n}?` from m to n, as few as possible
* **Special sequences**
  * `\A` start of string
  * `\b` matches empty string at word boundary (between `\w` and `\W`)
  * `\B` matches empty string not at word boundary
  * `\d` digit
  * `\D` non-digit
  * `\s` whitespace: `[ \t\n\r\f\v]`
  * `\S` non-whitespace
  * `\w` alphanumeric: `[0-9a-zA-Z_]`
  * `\W` non-alphanumeric
  * `\Z` end of string
  * `\g<id>` matches a previously defined group
* **Extensions**
  * `(?iLmsux)` Matches empty string, sets re.X flags
  * `(?:...)` Non-capturing version of regular parentheses
  * `(?P<name>...)` Creates a named capturing group
  * `(?P=name)` Matches whatever matched previously named group
  * `(?#...)` A comment; ignored.
  * `(?=...)` Lookahead assertion: Matches without consuming
  * `(?!...)` Negative lookahead assertion
  * `(?<=...)` Lookbehind assertion: Matches if preceded
  * `(?<!...)` Negative lookbehind assertion
  * `(?(id)yes|no)` Match 'yes' if group 'id' matched, else 'no'
