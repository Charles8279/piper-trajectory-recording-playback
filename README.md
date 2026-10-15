# Piper 机械臂轨迹记录与播放

记录松灵 Piper 机械臂连续轨迹记录与播放的学习笔记，重点整理 CSV 轨迹文件的保存、命名与播放管理。

## 官方项目

轨迹记录与播放功能基于松灵机器人官方示例学习与实践。

**官方代码：** [Agilex-College — recordAndPlayTraj](https://github.com/agilexrobotics/Agilex-College/tree/master/piper/recordAndPlayTraj)

具体实现、运行方法及相关依赖请参考官方仓库。

## CSV 轨迹文件管理

### 1. 保存多组测试轨迹

通过修改轨迹记录程序中的 CSV 文件名，将不同测试的轨迹分别保存，避免后续测试覆盖之前的数据。

示例：

- `trajectory_test_01.csv`
- `trajectory_test_02.csv`
- `trajectory_test_03.csv`

### 2. 选择需要播放的轨迹

播放时，通过修改播放程序中指定的 CSV 文件名，选择对应的轨迹文件。

例如，将读取路径设置为 `trajectory_test_02.csv`，即可指定第二组测试轨迹。

### 3. 文件管理建议

- 使用有意义的文件名区分不同测试。
- 记录每份 CSV 对应的动作、测试条件和运行结果。
- 播放前检查文件路径与数据格式。
- 重要测试数据及时备份，避免误覆盖。

## 说明

本仓库主要用于个人学习笔记与 CSV 文件管理经验整理。机械臂控制程序及其具体实现请以松灵机器人官方仓库为准。# piper-trajectory-recording-playback
Continuous trajectory recording and playback for the AgileX Piper robotic arm. 
