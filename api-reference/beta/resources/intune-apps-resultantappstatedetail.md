---
title: resultantAppStateDetail 枚举类型
description: 枚举指示其他详细信息有关为什么应用程序具有特定安装状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34b4d885f9ed2a23669bc2e30c91de40af8d915b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410236"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

枚举指示其他详细信息有关为什么应用程序具有特定安装状态。

## <a name="members"></a>成员
|成员|值|说明|
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




