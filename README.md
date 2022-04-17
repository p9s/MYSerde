# Rust 过程宏 学习记录

1. 过程宏必须定义在一个独立的create中
2. 过程宏必须定义在lib库中, 不能定义在bin中
3. 在Cargo.toml 中添加[lib]节点, 并增加  proc-macro=true
4. 添加 proc-macro后, crate只能导出过程宏, 其它不呆导出


# 使用到的依赖包
1. proc_macro2  
    对 proc_macro 的封装
2. syn
    基于 proc_macro2 中暴露的 TokenStream API 来生成 AST, 提供 AST 操作
3. quote
    配合syn, 将 AST转回 TokenSteam


# 参考阅读
1. Rust 编译过程与宏展开

