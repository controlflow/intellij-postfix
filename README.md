IntelliJ IDEA Postfix Completion plugin
---------------------------------------

The basic idea is to prevent caret jumps backward while typing code,
let you start with the some expression, explore some APIs, think about
what you are going to do and after finish with statement of some type.

#### Examples
![options](/content/example.png)

See [more examples](examples.md).

#### Current state

This plugin became a [core part of IntelliJ IDEA 13.1 experience](http://blog.jetbrains.com/idea/2014/03/postfix-completion/)!
Source code is no longer maintained here.

#### Download

Latest builds for IDEA 13 is available for download in [IntelliJ IDEA plugin repository](http://plugins.jetbrains.com/plugin/7342).
To install into IDEA simply go *Preferences* – *Plugins* – *Browse repositories...* and search for *"postfix"*.

#### Features

Available templates:

* `.if` – checks boolean expression to be true `if (expr)`
* `.else` – checks boolean expression to be false `if (!expr)`
* `.var` – initialize new variable with expression `T name = expr;`
* `.null` – checks nullable expression to be null `if (expr == null)`
* `.notnull` – checks expression to be non-null `if (expr != null)`
* `.instanceof` – checks type `expr instanceof T ? ((T) expr).m : null`
* `.not` – negates value of inner boolean expression `!expr`
* `.for` – iterates over collection `for (T item : collection)`
* `.while` – uses expression as loop condition `while (expr)`
* `.arg` – helps surround argument with invocation `method(expr)`
* `.cast` – surrounds expression with cast `(SomeType) expr`
* `.new` – produces instantiation expression for type `new T()`
* `.fori` – surrounds with loop `for (int i = 0; i < expr.length; i++)`
* `.forr` – reverse loop `for (int i = expr.length - 1; i >= 0; i--)`
* `.field` – introduces field for expression `_field = expr;`
* `.par` – surrounds outer expression with parentheses `(expr)`
* `.return` – returns value from containing method `return expr;`
* `.switch` – switch over integral/enum/string values `switch (expr)`
* `.throw` – throws exception of 'Throwable' type `throw new Exception();`
* `.assert` - creates assertion from boolean expression `assert expr;`
* `.synchronized` – produces synchronized block `synchronized (expr)`

Other features:

* Template expansion by `Tab` key in editor (like live templates)
* Settings page to disable/enable particular postfix templates

#### .NET version

* [Postfix Templates plugin for ReSharper](https://github.com/controlflow/resharper-postfix)