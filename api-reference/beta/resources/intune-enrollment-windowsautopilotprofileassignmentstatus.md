---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f4c6fbfcbefd88af31f2875cf33755b3be21e06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525276"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的工作分配状态|
|assignedInSync|1|在 Intune 中成功分配, 并与 Windows 自动试用程序同步|
|assignedOutOfSync|2 |已在 Intune 中成功分配, 与 Windows 自动试用程序不同步|
|assignedUnkownSyncState|3 |在 Intune 中成功分配, 并与 Windows 自动试用程序同步或不同步|
|notAssigned|4 |未分配|
|决|5 |挂起分配|
|未能|6 | 分配失败|





