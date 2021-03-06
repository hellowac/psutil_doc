# Summary

[说明](./readme.md)

----

# 中文

- [指南](guide/readme.md)
  - [快速连接](guide/quick_link.md)
  - [关于](guide/about.md)
- [基金](guide/funding.md)
- [安装](guide/install.md)
- [系统](system/readme.md)
  - [CPU](system/cpu/readme.md)
    - [执行时间](system/cpu/cpu_times.md)
    - [利用率](system/cpu/cpu_percent.md)
    - [利用率详细](system/cpu/cpu_times_percent.md)
    - [核心数量](system/cpu/cpu_count.md)
    - [统计信息](system/cpu/cpu_stats.md)
    - [频率信息](system/cpu/cpu_freq.md)
    - [负载信息](system/cpu/getloadavg.md)
  - [内存](system/memory/readme.md)
    - [运行内存](system/memory/virtual_memory.md)
    - [交换内存](system/memory/swap_memory.md)
  - [磁盘](system/disks/readme.md)
    - [挂载信息](system/disks/disk_partitions.md)
    - [利用率](system/disks/disk_usage.md)
    - [IO统计](system/disks/disk_io_counters.md)
  - [网络](system/network/readme.md)
    - [网络统计信息](system/network/net_io_counters.md)
    - [网络连接信息](system/network/net_connections.md)
    - [网络连接信息](system/network/net_if_addrs.md)
    - [网卡状态](system/network/net_if_stats.md)
  - [传感器](system/Sensors/readme.md)
    - [温度](system/Sensors/sensors_temperatures`.md)
    - [风扇](system/Sensors/sensors_fans.md)
    - [电池](system/Sensors/sensors_battery.md)
  - [其他系统信息](system/other/readme.md)
    - [启动时间](system/other/boot_time.md)
    - [用户](system/other/users.md)
- [进程](processes/readme.md)
  - [函数](processes/functions/readme.md)
    - [进程ID列表](processes/functions/pids.md)
    - [迭代进程](processes/functions/process_iter.md)
    - [检查进程是否存在](processes/functions/pid_exists.md)
    - [等待进程终止](processes/functions/wait_procs.md)
  - [异常](processes/exceptions/readme.md)
  - [进程类](processes/process_class/readme.md)
    - [快照](processes/process_class/oneshot.md)
    - [进程ID](processes/process_class/pid.md)
    - [父进程ID](processes/process_class/ppid.md)
    - [进程名称](processes/process_class/name.md)
    - [可执行文件绝对路径](processes/process_class/exe.md)
    - [执行命令行](processes/process_class/cmdline.md)
    - [环境变量](processes/process_class/environ.md)
    - [创建时间](processes/process_class/create_time.md)
    - [字典信息](processes/process_class/as_dict.md)
    - [父进程](processes/process_class/parent.md)
    - [父进程列表](processes/process_class/parents.md)
    - [进程状态](processes/process_class/status.md)
    - [执行目录](processes/process_class/cwd.md)
    - [所属用户名](processes/process_class/username.md)
    - [用户ID](processes/process_class/uids.md)
    - [组ID](processes/process_class/gids.md)
    - [终端](processes/process_class/terminal.md)
    - [优先级](processes/process_class/nice.md)
    - [I/O优先级](processes/process_class/ionice.md)
    - [资源限制](processes/process_class/rlimit.md)
    - [I/O统计](processes/process_class/io_counters.md)
    - [上下文切换数](processes/process_class/num_ctx_switches.md)
    - [文件描述符数](processes/process_class/num_fds.md)
    - [句柄数](processes/process_class/num_handles.md)
    - [线程数](processes/process_class/num_threads.md)
    - [线程](processes/process_class/threads.md)
    - [cpu时间](processes/process_class/cpu_times.md)
    - [cpu利用率](processes/process_class/cpu_percent.md)
    - [cpu亲和度](processes/process_class/cpu_affinity.md)
    - [cpu数量](processes/process_class/cpu_num.md)
    - [内存信息](processes/process_class/memory_info.md)
    - [memory_info_ex]()
    - [内存完全信息](processes/process_class/memory_full_info.md)
    - [内存利用率](processes/process_class/memory_percent.md)
    - [内存映射](processes/process_class/memory_maps.md)
    - [子进程](processes/process_class/children.md)
    - [打开的文件](processes/process_class/open_files.md)
    - [网络连接](processes/process_class/connections.md)
    - [是否正在运行](processes/process_class/is_running.md)
    - [发送信号](processes/process_class/send_signal.md)
    - [暂停进程](processes/process_class/suspend.md)
    - [恢复进程](processes/process_class/resume.md)
    - [终止进程](processes/process_class/terminate.md)
    - [杀死进程](processes/process_class/kill.md)
    - [等待](processes/process_class/wait.md)
    - [进程管道](processes/process_class/popen.md)
- [Windows 服务](windows_services/readme.md)
  - [迭代服务](windows_services/win_service_iter.md)
  - [根据名称获取服务](windows_services/win_service_get.md)
  - [win服务类](windows_services/windows_service.md)
- [常量](constants/readme.md)
  - [操作系统](constants/op_system.md)
  - [进程状态](constants/process_status.md)
  - [进程优先级](constants/process_priority.md)
  - [进程资源](constants/process_source.md)
  - [网络连接](constants/connections.md)
  - [硬件](constants/hardware.md)
- [工具函数](recipes/readme.md)
  - [按名称查找进程](recipes/find_process_by_name.md)
  - [终止进程树](recipes/kill_process_tree.md)
  - [过滤和排序进程](recipes/filter_and_sort_process.md)
  - [字节转换](recipes/bytes_conversion.md)
- [常见问题](faqs/readme.md)
- [测试](tests/readme.md)
- [安全](security/readme.md)
- [开发指南](deveplotment/readme.md)
- [平台支持历史](history/readme.md)
- [时间线](timeline/readme.md)
