# 审核触发器

使用 PostgreSQL 的触发器功能来创建一个审核触发器示例

## 步骤

创建 notify_test 数据库，然后执行 audit_tigger.sql 初始化数据库

进入 psql shell 开始测试

```
INSERT INTO notify_test VALUES (1);
UPDATE notify_test SET i = 2;
DELETE FROM notify_test;

SELECT * FROM audit_log;
```
