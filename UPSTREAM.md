# 源码来源

jsrv8 派生自 https://github.com/neverl805/never-jscore 。

基线提交：`cb00a6fb3e15cc42f015e8e8b83bfdea26760224`，上游版本 3.2.0。
原作者及版权归属保留为 never_jscore contributors；上游 Cargo.toml、
pyproject.toml 和 src/permissions.rs 声明 MIT 许可证。

本项目初始修改：发行名与 Python 导入名改为 jsrv8，不默认编译内置 Canvas。
Web API 与其内部 Node 模块依赖一起编译；运行时不默认启用 Node 全局兼容。
原 API Context / JSEngine 保留。
本项目不是上游官方发行，平台支持以实际发布并验证的 wheel 为准。
