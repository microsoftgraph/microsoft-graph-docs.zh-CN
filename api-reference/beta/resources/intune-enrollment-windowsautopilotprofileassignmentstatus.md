---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b5d1af0e6c91dced1aa12ae72c22430d16674c21
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156376"
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
|assignedOutOfSync|双面|已在 Intune 中成功分配, 与 Windows 自动试用程序不同步|
|assignedUnkownSyncState|第三章|在 Intune 中成功分配, 并与 Windows 自动试用程序同步或不同步|
|notAssigned|4|未分配|
|决|5|挂起分配|
|failed|型| 分配失败|




