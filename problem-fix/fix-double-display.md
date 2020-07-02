# Ubuntu不同分辨率双屏显示问题

* 显示有哪些设备

  ```bash
  xrandr
  ```

* 将1080p分辨率的屏幕设置为与4K屏分辨率相同

  ```bash
  xrandr --output DP-2 --scale 2x2
  ```

* 设置1080p分辨率的屏幕翻转、位置拖动
 ```bash
  nvidia-settings
 ```

* 在系统设置中将显示调为200%