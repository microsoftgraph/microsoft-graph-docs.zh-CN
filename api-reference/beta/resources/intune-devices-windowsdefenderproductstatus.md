---
title: windowsDefenderProductStatus 枚举类型
description: Windows Defender 的产品状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0485dd4b375206d08ba0c744d0b0c3fca09b12c0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241262"
---
# <a name="windowsdefenderproductstatus-enum-type"></a>windowsDefenderProductStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows Defender 的产品状态

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noStatus|0|无状态|
|serviceNotRunning|1|服务未运行|
|serviceStartedWithoutMalwareProtection|双面|服务启动时没有任何恶意软件保护引擎|
|pendingFullScanDueToThreatAction|4 |由于威胁操作而要等待完全扫描|
|pendingRebootDueToThreatAction|8 |由于威胁操作而等待重新启动|
|pendingManualStepsDueToThreatAction|16 |由于威胁操作而挂起的手动步骤 |
|avSignaturesOutOfDate|32|AV 签名已过期|
|asSignaturesOutOfDate|64|当签名过期时|
|noQuickScanHappenedForSpecifiedPeriod|128|在指定时间段内未发生快速扫描|
|noFullScanHappenedForSpecifiedPeriod|256|在指定时间段内未发生完全扫描|
|systemInitiatedScanInProgress|512|系统启动的扫描正在进行|
|systemInitiatedCleanInProgress|1024|系统启动的清理正在进行|
|samplesPendingSubmission|2048|有一些示例正在等待提交|
|productRunningInEvaluationMode|4096|以评估模式运行的产品|
|productRunningInNonGenuineMode|8192|在非正版 Windows 模式下运行的产品|
|productExpired|16384|产品已过期|
|offlineScanRequired|32768|需要离线扫描|
|serviceShutdownAsPartOfSystemShutdown|65536|服务在系统关闭过程中关闭|
|threatRemediationFailedCritically|131072|威胁修正失败严重|
|threatRemediationFailedNonCritically|262144|威胁补救失败不严重|
|noStatusFlagsSet|524288|状态标志设置 (初始化良好状态) |
|platformOutOfDate|1048576|平台已过期|
|platformUpdateInProgress|2097152|正在进行平台更新|
|platformAboutToBeOutdated|4194304|即将过期的平台|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|签名或平台寿命结束或即将过期|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|在非 Win10S 安装中仍在使用 Windows SMode 签名|




