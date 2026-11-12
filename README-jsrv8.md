# jsrv8

基于 never-jscore 的 Python 内嵌 V8 运行时，发行名称和导入名称均为 `jsrv8`。

```python
import jsrv8

ctx = jsrv8.Context(enable_extensions=True)
print(ctx.eval("Promise.resolve(42)", return_value=True))
del ctx
```

安装：`pip install jsrv8`。平台支持以 PyPI 实际 wheel 列表为准。

本项目保留上游 `Context` 和 `JSEngine` 接口。编译包含 Web API 必需的内部
Node 模块，默认不开启用户可见的 Node 兼容环境。Canvas 可使用外接 CanvasKit。
这不是浏览器安全沙箱，不应执行不可信代码。

源码来源及修改说明见 [UPSTREAM.md](UPSTREAM.md)，许可证见 [LICENSE](LICENSE)。
