# logsys
日志数据或内存数据的格式化输出系统，主要包括info、debug、warn、error、dump等。

**示例代码：**

```c
info("This a log for information");
debug("This a log for debuging");
warn("This a log for warning");
error("This a log for error");
dump("example", example, 100);
```

**示例日志：**

```txt
/f/project/example/src/example.c:14, main(), <info>, This a log for information
/f/project/example/src/example.c:15, main(), <debug>, This a log for information
/f/project/example/src/example.c:16, main(), <warn>, This a log for information
/f/project/example/src/example.c:17, main(), <error>, This a log for information
/f/project/example/src/example.c:18, main(), <dump>, [example]: length = 100 (0x64)

    0x100403020  54 68 69 73 20 69 73 20 - 61 20 65 78 61 6D 70 6C         | This is a exampl
    0x100403030  65 20 66 6F 72 20 6C 6F - 67 73 79 73 2E 00 00 00         | e for logsys....
    0x100403040  00 00 00 00 00 00 00 00 - 00 00 00 00 00 00 00 00         | ................
    0x100403050  00 00 00 00 00 00 00 00 - 00 00 00 00 00 00 00 00         | ................
    0x100403060  00 00 00 00 00 00 00 00 - 00 00 00 00 00 00 00 00         | ................
    0x100403070  00 00 00 00 00 00 00 00 - 00 00 00 00 00 00 00 00         | ................
    0x100403080  00 00 00 00             -                                 | ....
```

