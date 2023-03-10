## AtriBot

基于 OpenAI 的 TextCompletion API 实现的 AI 对话机器人。

### 编译环境

- ubuntu 22.04

### 编译前的准备

- 需要在根目录中新建一个文件 `initKey.h` ，在其中使用 OpenAI 的API key 定义 `API_KEY`。
- 安装vcpkg并导入如下的第三方库
  - HTTP 库： [C++ Requests](https://github.com/libcpr/cpr)
  - JSON 库：[JSON for Modern C++](https://github.com/nlohmann/json)



### 开发日志

- 2023/03/07

  实现多人聊天。用 `string_view` 替换了 `const string&` 。

- 2023/03/06

  实现一个简单的 Logger 用以调试。实现 ChatBot 的第一个版本。

- 2023/03/05

  重构 ChatCache。

- 2023/03/04

  设计并优化了 ChatBot 的基本框架。

- 2023/03/02

  对 OpenAI 的 API 进行基本的封装。统一调用返回时的格式。编写 TestBot 以测试封装库的正确性。

