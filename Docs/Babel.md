# Babel
> Babel 是一个工具链，主要用于将 ECMAScript 2015+ 版本的代码转换为向后兼容的 JavaScript 语法，以便能够运行在当前和旧版本的浏览器或其他环境中

Babel转换源码分为三个步骤:
- 解析（parse）： 进行词法分析（Lexical Analysis）和语法分析（Syntactic Analysis）以生成抽象语法树（AST）；
- 转换 (transform)： 遍历AST中每个节点并进行相应的转换操作，该过程通过使用不同的插件来实现各种特性和语法的转换；
- 生成 (generate)： 根据AST生成目标代码
