sql-log-proxy
==================

作为MySQL(TCP)代理，对客户端执行的sql语句进行记录；用于回溯、审计、日志、云迁移等场景。


使用方法举例
------------

代理端启动不限IP方式：

./sql-log-proxy -backend="127.0.0.1:3306" -bind=":3307" --verbose


代理端启动限制IP方式：

./sql-log-proxy -backend="127.0.0.1:3306" -bind="127.0.0.1:3307" --verbose


鸣谢
------------
原始版本基于 https://github.com/arstercz/portproxy