# Rust 过程宏 学习记录

1. 过程宏必须定义在一个独立的create中
2. 过程宏必须定义在lib库中, 不能定义在bin中
3. 在Cargo.toml 中添加[lib]节点, 并增加  proc-macro=true
4. 添加 proc-macro后, crate只能导出过程宏, 其它不呆导出

