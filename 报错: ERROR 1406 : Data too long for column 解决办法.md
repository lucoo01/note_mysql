## ERROR 1406 : Data too long for column 解决办法

### 解决办法:

在my.ini里找到
```
sql-mode=”STRICT_TRANS_TABLES,NO_AUTO_Create_USER,NO_ENGINE_SUBSTITUTION”
```
把其中的STRICT_TRANS_TABLES,去掉,

或者把`sql-mode=STRICT_TRANS_TABLES,NO_AUTO_Create_USER,NO_ENGINE_SUBSTITUTION`

注释掉，然后重启mysql就ok了
