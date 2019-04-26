# 任务要求
- 用bash编写一个文本批处理脚本，对以下附件分别进行批量处理完成相应的数据统计任务
	- [2014世界杯运动员数据](http://sec.cuc.edu.cn/huangwei/course/LinuxSysAdmin/exp/chap0x04/worldcupplayerinfo.tsv)
		- 统计不同年龄区间范围（20岁以下、[20-30]、30岁以上）的球员数量、百分比
		- 统计不同场上位置的球员数量、百分比
		- 名字最长的球员是谁？名字最短的球员是谁？
		- 年龄最大的球员是谁？年龄最小的球员是谁？

# 实施过程
- 根据题意, 处理脚本不需要编写成`shell tool`, 只要能得出统计结果即可
- 任务本身并不难, 只需逐行读取目标文件, 在条件符合时将相应的变量`+=1`即可

# 统计结果
```
总共有736位球员. 其中:
  20岁以下的球员有9位, 占比1.22%
  20~30岁以下的球员有600位, 占比81.52%
  30岁以上的球员有127位, 占比17.25%
  defender有237位, 占比32.20%
  forward有135位, 占比18.34%
  goalie有96位, 占比13.04%
  midfielder有268位, 占比36.41%
  名字最短的球员是Jô, 其名字长度为2
  名字最长的球员是Francisco_Javier_Rodriguez, 其名字长度为26
  最年轻的球员是Fabrice_Olinga, 年龄18
  最年长的球员是Faryd_Mondragon, 年龄42
```