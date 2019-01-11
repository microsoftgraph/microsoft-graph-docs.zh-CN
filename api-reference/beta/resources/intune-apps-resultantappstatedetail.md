---
title: resultantAppStateDetail 枚举类型
description: 枚举指示其他详细信息有关为什么应用程序具有特定安装状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5c5eb8c921be7c14a45c979a57ffcaa0704d9b4b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874142"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

枚举指示其他详细信息有关为什么应用程序具有特定安装状态。
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|noAdditionalDetails|0|可用不的任何其他的详细信息。|
|seeInstallErrorCode|2000|应用程序安装失败。 请参阅错误代码的详细信息的属性。|
|seeUninstallErrorCode|4000|应用程序卸载失败。 请参阅错误代码的详细信息的属性。|
|pendingReboot|5000|必须重新启动设备，以完成安装的应用程序。|
|platformNotApplicable|-1006|应用程序不适用于此平台。 （例如 Android 应用程序针对 IOS）|
|minimumCpuSpeedNotMet|-1005|配置最小值小于目标设备上的 CPU 速度。|
|minimumLogicalProcessorCountNotMet|-1004|配置最小值小于目标设备上的逻辑处理器的计数。|
|minimumPhysicalMemoryNotMet|-1003|目标设备上的 RAM 量小于配置的最小值。|
|minimumOsVersionNotMet|-1002|配置最小值小于目标设备上的操作系统版本。|
|minimumDiskSpaceNotMet|-1001|目标设备上的可用磁盘空间小于配置的最小值。|
|processorArchitectureNotApplicable|-1000|设备体系结构 (如 x86/amd64) 不适用的应用程序。|





