# STM32F103 Timer PWM

STM32F103C8T6（Blue Pill）+ STM32CubeMX + Keil MDK5 + HAL 库的定时器 PWM 实验。

## 项目

| 目录 | 内容 |
| --- | --- |
| `Task1_Timer_LED_2s` | TIM3 更新中断控制 LED，亮 1 s、灭 1 s，完整周期 2 s |
| `Task2_PWM_Breathing` | TIM3_CH1（PA6）PWM 呼吸灯，约 2 s 一个周期 |

## 硬件

- STM32F103C8T6 最小系统板
- ST-Link V2
- LED 接 PA6（TIM3_CH1）
- 系统时钟：HSI 8 MHz

## 开发环境

- STM32CubeMX
- Keil MDK5（ARM Compiler 6）
- STM32Cube FW_F1 固件包
- HAL 库

## 打开方式

用 Keil 打开对应工程目录下的 `MDK-ARM/*.uvprojx`：

- `Task1_Timer_LED_2s/MDK-ARM/Timer_LED_2s.uvprojx`
- `Task2_PWM_Breathing/MDK-ARM/PWM_Breathing.uvprojx`

CubeMX 工程文件为对应目录下的 `.ioc`。

## 说明

仓库只保存源码和工程配置，不包含 `Objects`、`Listings`、`.axf`、`.hex` 等编译产物。
