# 什么是 WebMCP 以及它能做什么？

参考官方文档：[WebMCP Explainer](https://docs.google.com/document/d/1rtU1fRPS0bMqd9abMG_hc6K9OAI6soUy3Kh00toAgyk/edit?tab=t.0)

以下是 WebMCP 应用于网站的一些示例：

- 某航空公司的网站暴露了一个 `book_flight` 工具。AI Agent 可以直接通过该工具提交结构化的乘客数据，而不必去猜测该如何在航空公司那个为人类用户设计的日历 UI 上进行输入。

- 复杂的医疗或法律门户网站将表单标注为 `submit_application` 工具。Agent 可以正确且即时地将数据映射到对应字段，而不会把数据重复填入错误的字段。例如，可以明确指示某个字段需要填写完整的法定姓名，还是分开的姓和名字段。

- 开发者设置页面暴露了一个 `run_diagnostics` 工具，这样 Agent 就能直接触发诊断修复操作，而这些操作原本隐藏在层层嵌套的菜单之后。

简单来说，WebMCP 的核心思路就是：让网站主动把自己的能力以"工具"的形式暴露给 AI Agent，这样 Agent 就不用像人一样去"看"页面、"猜"交互方式，而是直接通过结构化的接口完成操作，既准确又高效。

# 怎么才能用？

## 浏览器版本要求

需要 Chrome **Version 146.0.7672.0** 或更高版本。

## 下载地址

直接上金丝雀版：<https://www.google.com/intl/en/chrome/canary/>

## 开启 Feature Flag

参考文档：[Chrome Flags 说明](https://developer.chrome.com/docs/web-platform/chrome-flags?hl=zh-cn)

步骤：

1. 地址栏输入 `chrome://flags/`
2. 搜索 `webmcp`
3. 将对应开关设为 **Enabled**

![WebMCP Feature Flag 开关示意](web_mcp_flag.png)