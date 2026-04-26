# ALC16P

English: see [Overview](#overview)  
Русский: см. [Описание на русском](#описание-на-русском)

## Overview

ALC16P is an ESP32-based 16-channel PWM controller for DIY LED fixtures.

It is primarily intended for:
- marine aquariums
- freshwater aquariums
- indoor plant growing

The controller is designed for fully offline operation:
- no Internet connection required
- no cloud services
- no subscription dependency

### Main functions

- 16 independent PWM channels for LED lighting
- daily schedule control
- daily schedule helper:
  - 4-point trapezoidal mode
  - 16-point sinusoidal mode
  - available globally for all channels and individually per channel
- schedule synchronization between multiple controllers
- DS18B20-based temperature monitoring
- heating/cooling control by temperature
- LED overheat protection with automatic brightness reduction when LED heatsink temperature is exceeded
- DS3231 RTC support
- timers
- dosing timers with calculation helper
- important status information on a small SSD1306 OLED display
- local web interface over Wi-Fi with HTTPS
- OTA firmware update

### Typical use

The project is intended for building custom LED fixtures where the user wants direct control over channels, schedules, and local automation without external infrastructure.

## Описание на русском

ALC16P — это 16-канальный PWM-контроллер на базе ESP32 для DIY LED светильников.

Основные области применения:
- морской аквариум
- пресноводный аквариум
- домашнее выращивание растений

Контроллер рассчитан на полностью автономную локальную работу:
- подключение к Internet не требуется
- зависимости от облачных сервисов нет
- платные подписки не нужны

### Основные функции

- 16 независимых PWM каналов для управления светом
- управление суточными графиками
- помощник построения суточных графиков:
  - 4 точки — трапецеидальный режим
  - 16 точек — синусоидальный режим
  - доступен как для всех каналов сразу, так и индивидуально для каждого канала
- синхронизация графиков между несколькими контроллерами
- работа с температурными датчиками DS18B20
- управление нагревом и охлаждением по температуре
- обработка аварий по перегреву LED с автоматическим снижением светимости каналов при превышении температуры радиатора(ов) светильника
- поддержка RTC DS3231
- таймеры
- таймеры дозирования с расчетным помощником
- вывод важной информации на мини-дисплей SSD1306 OLED
- локальный web-интерфейс по Wi‑Fi с HTTPS
- OTA обновление прошивки

### Назначение

Проект предназначен для самостоятельной сборки LED светильников с локальным управлением, расписаниями и автоматикой без внешней инфраструктуры.
