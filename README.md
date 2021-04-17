# 如何调试存储过程
## 由于我在 13/data/postgresql.conf 这个文件里开启了'plugin_debugger'：
```postgresql
shared_preload_libraries = 'plugin_debugger'

```
## 在需要调试存储过程的目标数据库中，安装pldbgapi插件

### 指定某个数据库执行：

```postgresql

create extension pldbgapi;

```