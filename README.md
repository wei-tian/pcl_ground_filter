ray地面滤除
---
## 依赖
需要pcl1.7

## 输入输出
接收bin二进制文件输入(单个文件或者保存bin文件的文件夹),二进制文件的格式为:
[x,y,z,*,*,x,y,z,*,*..........x,y,z,*,*], 元素为float.
即5个一组表示一个点,循环排列.

输出有三个:
1. 原始bin文件转换成的点云pcd
2. 滤除地面后的点云保存成的pcd
3. 滤除地面后的点云保存成的二进制bin文件,格式为[x,y,z,x,y,z.....x,y,z], 元素为float

## 使用
1. 编译
2. 建立config.ini文件,并和ground_filter可执行文件放在一起.(config文件参考config.ini)
3. 运行
`./ground_filter <bin文件/文件夹> <输出文件夹>`


