# 资源限制

**Process.rlimit(resource, limits=None)** - [原文](https://psutil.readthedocs.io/en/latest/#psutil.Process.rlimit) <a name="Process.rlimit" ></a>

读写进程资源限制(参见 [prlimit][prlimit] 手册)。 ***resource*** 是 [psutil.RLIMIT_*](#process-resources-const)常量之一。 ***limits*** 是一个 `(soft, hard)` 元组。本函数作用与 [resource.getrlimit][resource.getrlimit] 和 [resource.getrlimit][resource.getrlimit] 一样，不过本函数可以作用于任何进程PID，不仅仅是 [os.getpid][os.getpid]所获取的 。读时，返回值是一个 `(soft, hard)` 元组。每个值可以是 整数 或 [psutil.RLIMIT_*](#process-resources-const)。 例子：

[prlimit]: https://linux.die.net/man/2/prlimit "prlimit"
[resource.getrlimit]: https://docs.python.org/3/library/resource.html#resource.getrlimit  "resource.getrlimit"
[resource.setrlimit]: https://docs.python.org/3/library/resource.html#resource.setrlimit  "resource.setrlimit"
[procinfo.py]: https://github.com/giampaolo/psutil/blob/master/scripts/procinfo.py "procinfo.py"

```python
>>> import psutil
>>> p = psutil.Process()
>>> p.rlimit(psutil.RLIMIT_NOFILE, (128, 128))   # process can open max 128 file descriptors
>>> p.rlimit(psutil.RLIMIT_FSIZE, (1024, 1024))  # can create files no bigger than 1024 bytes
>>> p.rlimit(psutil.RLIMIT_FSIZE)                # get
(1024, 1024)
>>>
```

同样参考 [procinfo.py][procinfo.py] 脚本

*可用平台: Linux, FreeBSD.*

*5.7.3 版本中修改: 新增 FreeBSD 支持。*
