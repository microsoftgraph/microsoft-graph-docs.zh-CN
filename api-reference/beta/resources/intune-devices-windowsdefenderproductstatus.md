---
title: windowsDefenderProductStatus 枚举类型
description: 产品状态Windows Defender
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a126fb37736d8d02accdd9b3dc0eff8cacf7173
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59046860"
---
# <a name="windowsdefenderproductstatus-enum-type"></a>windowsDefenderProductStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

产品状态Windows Defender

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|noStatus|0|无状态|
|serviceNotRunning|1|服务未运行|
|serviceStartedWithoutMalwareProtection|2|无需任何恶意软件保护引擎即可启动服务|
|pendingFullScanDueToThreatAction|4 |由于威胁操作而挂起完全扫描|
|pendingRebootDueToThreatAction|8 |由于威胁操作而挂起重启|
|pendingManualStepsDueToThreatAction|16 |由于威胁操作而挂起的手动步骤 |
|avSignaturesOutOfDate|32|AV 签名过期|
|asSignaturesOutOfDate|64|AS 签名过期|
|noQuickScanHappenedForSpecifiedPeriod|128|指定时段内未发生快速扫描|
|noFullScanHappenedForSpecifiedPeriod|256|指定的时段内未发生完全扫描|
|systemInitiatedScanInProgress|512|正在进行系统启动的扫描|
|systemInitiatedCleanInProgress|1024|正在进行清理的系统启动|
|samplesPendingSubmission|2048|有一些等待提交的示例|
|productRunningInEvaluationMode|4096|在评估模式下运行的产品|
|productRunningInNonGenuineMode|8192|在非正版正版Windows运行的产品|
|productExpired|16384|产品已过期|
|offlineScanRequired|32768|需要外线扫描|
|serviceShutdownAsPartOfSystemShutdown|65536|服务正在关闭，作为系统关闭的一部分|
|threatRemediationFailedCritically|131072|威胁修正严重失败|
|threatRemediationFailedNonCritically|262144|威胁修正失败（非严重）|
|noStatusFlagsSet|524288|没有为初始化 (状态设置状态) |
|platformOutOfDate|1048576|平台已过期|
|platformUpdateInProgress|2097152|平台更新正在进行中|
|platformAboutToBeOutdated|4194304|平台即将过时|
|signatureOrPlatformEndOfLifeIsPastOrIsImpending|8388608|签名或平台生命周期已过去或即将结束|
|windowsSModeSignaturesInUseOnNonWin10SInstall|16777216|WindowsSMode 签名仍在非 Win10S 安装上使用|



