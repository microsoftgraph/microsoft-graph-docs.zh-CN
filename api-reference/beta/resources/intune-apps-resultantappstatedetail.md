---
title: resultantAppStateDetail 枚举类型
description: 指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8d6b7e6a665229d02033cd1c0c25469a83dfc37d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167212"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAdditionalDetails|0|没有可用的其他详细信息。|
|seeInstallErrorCode|2000|应用程序安装失败。 有关更多详细信息, 请参阅错误代码属性。|
|seeUninstallErrorCode|4000|应用程序卸载失败。 有关更多详细信息, 请参阅错误代码属性。|
|pendingReboot|5000|必须重新启动设备才能完成应用程序的安装。|
|platformNotApplicable|-1006|应用程序不适用于此平台。 (例如, 面向 IOS 的 Android 应用)|
|minimumCpuSpeedNotMet|-1005|目标设备上的 CPU 速度小于配置的最小值。|
|minimumLogicalProcessorCountNotMet|-1004|目标设备上的逻辑处理器计数小于配置的最小值。|
|minimumPhysicalMemoryNotMet|-1003|目标设备上的 RAM 量小于配置的最小值。|
|minimumOsVersionNotMet|-1002|目标设备上的 OS 版本小于配置的最小值。|
|minimumDiskSpaceNotMet|-1001|目标设备上的可用磁盘空间小于配置的最小值。|
|processorArchitectureNotApplicable|-1000|设备体系结构 (例如, x86/amd64) 不适用于应用程序。|




