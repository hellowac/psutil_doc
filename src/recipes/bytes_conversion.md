# 字节转换

参考: [原文](https://psutil.readthedocs.io/en/latest/#bytes-conversion)

```python
import psutil

def bytes2human(n):
    # http://code.activestate.com/recipes/578019
    # >>> bytes2human(10000)
    # '9.8K'
    # >>> bytes2human(100001221)
    # '95.4M'
    symbols = ('K', 'M', 'G', 'T', 'P', 'E', 'Z', 'Y')
    prefix = {}
    for i, s in enumerate(symbols):
        prefix[s] = 1 << (i + 1) * 10
    for s in reversed(symbols):
        if n >= prefix[s]:
            value = float(n) / prefix[s]
            return '%.1f%s' % (value, s)
    return "%sB" % n

total = psutil.disk_usage('/').total
print(total)
print(bytes2human(total))
```

…打印:

```python
100399730688
93.5G
```
