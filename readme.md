将 python 的 requests 代码转换成 curl 命令

# 安装

```python
pip install time_utils
```

# 使用

```python
from time_utils import TimeUtil

print(TimeUtil.get_current_time_str())  ###获取当前字符串格式化时间
print(TimeUtil.get_current_time_unix())  ###获取当前时间戳
print(TimeUtil.get_seven_days_ago_time_unix())
print(TimeUtil.str_time_to_unix("2022-07-07 20:28:50"))
print(TimeUtil.unix_time_to_str(1657197749260))
print(TimeUtil.get_recently_day(-7, 'unix'))
print(TimeUtil.get_day_begin_unix())
print(TimeUtil.get_day_end_unix(-4))
print(TimeUtil.get_month_datetime_begin(datetime.datetime.now()))
print(TimeUtil.get_month_datetime_end(datetime.datetime.now()))
print(TimeUtil.compare_time(datetime.datetime.fromisoformat('2022-07-01 00:00:00'),
                            datetime.datetime.fromisoformat('2022-05-31 23:59:59')))
```
