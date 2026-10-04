# gRPC 学习笔记

> gRPC 是 Google 开源的高性能 RPC 框架，基于 HTTP/2 + Protocol Buffers，是 Go 微服务间通信的事实标准。

## 本地内容

### lixueduan-gRPC系列教程/ —— 李学锻《gRPC(Go)系列教程》全文（14 篇）

来源：[lixd/blog](https://github.com/lixd/blog) 原始 Markdown，图片已全部本地化（`images/`）。

| # | 文章 | 主题 |
|---|------|------|
| 00 | [使用gRPC时遇到的问题](lixueduan-gRPC系列教程/00-使用gRPC时遇到的问题.md) | 入门前常见疑问 |
| 01 | [Protobuf](lixueduan-gRPC系列教程/01-Protobuf.md) | protoc 安装与 .proto 定义、编译 |
| 02 | [Hello-gRPC](lixueduan-gRPC系列教程/02-Hello-gRPC.md) | 第一个 gRPC 服务端/客户端 |
| 03 | [Stream推送流](lixueduan-gRPC系列教程/03-Stream推送流.md) | Unary / ServerStreaming / ClientStreaming / Bidirectional 四种 API |
| 04 | [SSL-TLS安全连接](lixueduan-gRPC系列教程/04-SSL-TLS安全连接.md) | TLS 证书 + openssl 制作证书 |
| 05 | [拦截器Interceptor](lixueduan-gRPC系列教程/05-拦截器Interceptor.md) | 一元/流式拦截器，go-grpc-middleware |
| 06 | [自定义身份校验](lixueduan-gRPC系列教程/06-自定义身份校验.md) | Token 认证 |
| 07 | [利用Gateway同时提供HTTP和RPC服务](lixueduan-gRPC系列教程/07-利用Gateway同时提供HTTP和RPC服务.md) | grpc-gateway 实战 |
| 08 | [context超时控制](lixueduan-gRPC系列教程/08-context超时控制.md) | Deadline / Cancel |
| 09 | [retry自动重试](lixueduan-gRPC系列教程/09-retry自动重试.md) | 重试策略配置 |
| 10 | [压测工具ghz](lixueduan-gRPC系列教程/10-压测工具ghz.md) | gRPC 压测 |
| 11 | [NameResolver实战及原理分析](lixueduan-gRPC系列教程/11-NameResolver实战及原理分析.md) | 服务发现原理 |
| 12 | [客户端负载均衡](lixueduan-gRPC系列教程/12-客户端负载均衡.md) | 客户端 LB 实战 |
| 13 | [K8S环境下的gRPC负载均衡](lixueduan-gRPC系列教程/13-K8S环境下的gRPC负载均衡.md) | headless service / envoy |

`code/grpc-go-example/` —— 系列教程配套示例代码（来自 [lixd/grpc-go-example](https://github.com/lixd/grpc-go-example)）。

### xinliangnote-gRPC笔记/ —— xinliangnote《Go 从入门到实战》gRPC 部分

- [Go gRPC Hello World](xinliangnote-gRPC笔记/01-Go%20gRPC%20Hello%20World.md)
- [Go gRPC 调试工具](xinliangnote-gRPC笔记/02-Go%20gRPC%20调试工具.md)

含可运行 codes（go_server / go_client），图片已本地化。

## 系统性中文教程（在线）

- 李文周 [gRPC教程](https://liwenzhou.com/posts/go/grpc/)（RPC 概念 + gRPC 完整入门）及系列：
  [RPC原理与Go RPC](https://liwenzhou.com/posts/go/rpc/) ·
  [Protobuf V3中文语法指南[翻译]](https://liwenzhou.com/posts/go/protobuf3-language-guide-zh/) ·
  [gRPC-Gateway使用指南](https://liwenzhou.com/posts/go/grpc-gateway/) ·
  [gRPC Transcoding](https://liwenzhou.com/posts/go/grpc-transcoding/) ·
  [gRPC中的名称解析和负载均衡](https://liwenzhou.com/posts/go/name-resolving-and-load-balancing-in-grpc/) ·
  [gRPC的链路追踪](https://liwenzhou.com/posts/go/go-grpc-otel/) ·
  [基于consul实现服务注册与发现](https://liwenzhou.com/posts/go/consul/)
- 李学锻《gRPC(Go)系列教程》目录页：https://www.lixueduan.com/categories/grpc/（即本目录 14 篇的在线版）
- 朱建斌《Go gRPC教程》12 篇（博客园，入门 5 篇 + 进阶 5 篇 + 负载均衡 2 篇）：https://github.com/Bingjian-Zhu/go-grpc-example（README 内有全部文章链接）

## 官方资源

- gRPC 官方文档（中文）：https://grpc.org.cn/docs/
- 官方文档（Go）：https://grpc.org.cn/docs/languages/go/
- grpc-go 源码与官方示例：https://github.com/grpc/grpc-go
- Protocol Buffers 下载与文档：https://github.com/protocolbuffers/protobuf
- 李文周代码示例：https://github.com/Q1mi/gRPC_demo

## 进阶：从零实现 RPC 框架

- 7 天用 Go 从零实现 RPC 框架 geeRPC（geektutu，配套免费在线教程）：https://github.com/geektutu/7days-golang
