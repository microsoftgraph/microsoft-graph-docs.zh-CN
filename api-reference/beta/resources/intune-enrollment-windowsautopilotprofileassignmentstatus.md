---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d241d93924de254af3cb76adfab27b49291b97f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941392"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的工作分配状态|
|assignedInSync|1|在 Intune 中成功分配, 并与 Windows 自动试用程序同步|
|assignedOutOfSync|双面|已在 Intune 中成功分配, 与 Windows 自动试用程序不同步|
|assignedUnkownSyncState|第三章|在 Intune 中成功分配, 并与 Windows 自动试用程序同步或不同步|
|notAssigned|4|未分配|
|决|5|挂起分配|
|未能|型| 分配失败|




