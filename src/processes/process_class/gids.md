# 组ID

**Process.gids()** - [原文](https://psutil.readthedocs.io/en/latest/#psutil.Process.gids) <a name="Process.gids" ></a>

返回一个由 (rgid, egid, sgid) 所组成的元组，分别表示当前进程的真实组ID，有效组ID和暂存组ID。这与 [os.getresgid][os.getresgid] 相同，但可用于任何进程 PID。

[os.getresgid]: https://docs.python.org/zh-cn/3/library/os.html#os.getresgid "os.getresgid"

*可用平台: UNIX。*
