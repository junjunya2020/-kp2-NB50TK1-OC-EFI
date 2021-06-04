# 时间校对问题
通常我们会添加系统时间补丁来解决这个问题，但是我们也可以通过简单的命令修改Windows 对硬件时间的对待方式来解决这个问题， 让 Windows 把硬件时间当作 UTC时间。

window7用户开始->运行->输入CMD

window8/10用户 WIN+x 选择管理员模式进入CMD

执行以下命令：

`Reg add HKLM\SYSTEM\CurrentControlSet\Control\TimeZoneInformation /v RealTimeIsUniversal /t REG_DWORD /d 1`

这样就不用添加系统时间补丁。
