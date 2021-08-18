---
title: resultantAppStateDetail 枚举类型
description: 指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4b83040763f0b7b56c4a6e8979a06f3f945a39ed94dde254c042648f8fe349f2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54250061"
---
# <a name="resultantappstatedetail-enum-type"></a>resultantAppStateDetail 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指示有关应用程序为何具有特定安装状态的其他详细信息的枚举。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noAdditionalDetails|0|没有可用的其他详细信息。|
|dependencyFailedToInstall|1 |无法安装应用程序的一个或多个依赖项。|
|dependencyWithRequirementsNotMet|2 |应用程序的一个或多个依赖项具有不满足的要求。|
|dependencyPendingReboot|3 |应用程序的一个或多个依赖项需要重新启动设备才能完成安装。|
|dependencyWithAutoInstallDisabled|4 |应用程序的一个或多个依赖项配置为不自动安装。|
|iosAppStoreUpdateFailedToInstall|1000|应用的最新版本无法从早期版本更新。|
|vppAppHasUpdateAvailable|1001|更新可用。|
|userRejectedUpdate|1002|用户拒绝了应用更新。 |
|seeInstallErrorCode|2000|应用程序安装失败。 有关详细信息，请参阅错误代码属性。|
|autoInstallDisabled|3000|应用程序配置为不自动安装。|
|managedAppNoLongerPresent|3001|应用已管理，但不再安装。|
|userRejectedInstall|3002|用户拒绝了应用安装。|
|userIsNotLoggedIntoAppStore|3003|用户必须登录到应用商店才能安装应用。|
|seeUninstallErrorCode|4000|应用程序无法卸载。 有关详细信息，请参阅错误代码属性。|
|pendingReboot|5000|必须重新启动设备才能完成应用程序的安装。|
|installingDependencies|5001|正在安装应用程序的一个或多个依赖项。|
|contentDownloaded|5002|应用程序内容已下载到设备。|
|powerShellScriptRequirementNotMet|-1013|不满足 PowerShell 脚本要求规则|
|registryRequirementNotMet|-1012|不满足注册表要求规则|
|fileSystemRequirementNotMet|-1011|不满足文件系统要求规则|
|platformNotApplicable|-1006|应用程序不适用于此平台。  (，例如面向 IOS 应用的 Android) |
|minimumCpuSpeedNotMet|-1005|目标设备的 CPU 速度小于配置的最小值。|
|minimumLogicalProcessorCountNotMet|-1004|目标设备上逻辑处理器的计数小于配置的最小处理器数。|
|minimumPhysicalMemoryNotMet|-1003|目标设备上 RAM 量小于配置的最小 RAM 量。|
|minimumOsVersionNotMet|-1002|目标设备上的操作系统版本小于配置的最低版本。|
|minimumDiskSpaceNotMet|-1001|目标设备的可用磁盘空间小于配置的最小磁盘空间。|
|processorArchitectureNotApplicable|-1000|设备体系结构 (例如 x86/amd64) 不适用于应用程序。|




