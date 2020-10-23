---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 93a956fa874fb50257da62fc9dbea59768e7a3cb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728905"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的工作分配状态|
|assignedInSync|1|在 Intune 中成功分配，并与 Windows 自动试用程序同步|
|assignedOutOfSync|双面|已在 Intune 中成功分配，与 Windows 自动试用程序不同步|
|assignedUnkownSyncState|第三章|在 Intune 中成功分配，并与 Windows 自动试用程序同步或不同步|
|notAssigned|4 |未分配|
|决|5 |挂起分配|
|未能|6 | 分配失败|





