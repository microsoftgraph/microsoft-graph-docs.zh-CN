---
title: resultantAppStateDetail 枚举类型
description: 指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c0de2345a4c698da79ec01db7bddcc139b5b2660
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43462538"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 枚举类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAdditionalDetails|0|没有可用的其他详细信息。|
|dependencyFailedToInstall|1|一个或多个应用程序的依存关系未能安装。|
|dependencyWithRequirementsNotMet|双面|一个或多个应用程序的依赖项具有未满足的要求。|
|dependencyPendingReboot|第三章|一个或多个应用程序的依赖项需要重新启动设备才能完成安装。|
|dependencyWithAutoInstallDisabled|4 |一个或多个应用程序的依赖项配置为不自动安装。|
|seeInstallErrorCode|2000|应用程序安装失败。 有关更多详细信息，请参阅错误代码属性。|
|autoInstallDisabled|3000|将应用程序配置为不会自动安装。|
|seeUninstallErrorCode|4000|应用程序卸载失败。 有关更多详细信息，请参阅错误代码属性。|
|pendingReboot|5000|必须重新启动设备才能完成应用程序的安装。|
|installingDependencies|5001|一个或多个应用程序的依赖项正在安装。|
|contentDownloaded|5002|将应用程序内容下载到设备。|
|powerShellScriptRequirementNotMet|-1013|不满足 PowerShell 脚本要求规则|
|registryRequirementNotMet|-1012|不符合注册表要求规则|
|fileSystemRequirementNotMet|-1011|不符合文件系统要求规则|
|platformNotApplicable|-1006|应用程序不适用于此平台。 （例如，面向 IOS 的 Android 应用）|
|minimumCpuSpeedNotMet|-1005|目标设备上的 CPU 速度小于配置的最小值。|
|minimumLogicalProcessorCountNotMet|-1004|目标设备上的逻辑处理器计数小于配置的最小值。|
|minimumPhysicalMemoryNotMet|-1003|目标设备上的 RAM 量小于配置的最小值。|
|minimumOsVersionNotMet|-1002|目标设备上的 OS 版本小于配置的最小值。|
|minimumDiskSpaceNotMet|-1001|目标设备上的可用磁盘空间小于配置的最小值。|
|processorArchitectureNotApplicable|-1000|设备体系结构（例如，x86/amd64）不适用于应用程序。|



