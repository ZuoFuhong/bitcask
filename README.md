## A simple key-value store

[TP 201: Practical Networked Applications in Rust](https://github.com/pingcap/talent-plan/blob/master/courses/rust/README.md) 构建一个单一的网络化、自定义协议、多线程和异步网络、持久键/值存储服务器和客户端。

### 知识点梳理

**Lesson 1**

1. 安装 Rust 以及工具链
2. 项目目录结构
3. 单元测试
4. 使用 `clap` crate 处理命令行参数。
5. 文档注释

**Lesson 2**

1. 错误处理, 使用 `failure` crate。
2. 结构化日志文件, 它与 `bitcask` 相同。

**Lesson 3**

1. 创建 client-server 应用程序。
2. 使用标准库的网络API 编写私有化协议。
3. 将日志记录引入服务器。
4. 实现具有 `trait` 的可拔插后端。
5. 将手写的 **KvStore** 与 `sled` 进行基准测试

**Lesson 4**

1. 服务端多线程处理请求（线程池）
2. 使用锁共享数据结构 `KvsEngine`
3. Lock-free readers（同一个文件可以打开多个句柄）

**Lesson 5**

1. 了解 Rust futures 使用模式。
2. 使用 tokio runtime 执行异步网络。
