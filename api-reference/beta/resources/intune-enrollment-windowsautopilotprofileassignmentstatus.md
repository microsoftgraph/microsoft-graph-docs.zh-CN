---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 48d08ad4d4c80c3d5a68cca5af36c958deaac819
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869641"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

尚未记录
## <a name="members"></a>成员
|成员|值|Description|
|:---|:---|:---|
|unknown|0|未知的工作分配状态|
|assignedInSync|1|分配 Intune 中成功的 Windows 自动试用计划同步|
|assignedOutOfSync|2|分配 Intune 中成功的不与同步 Windows 自动试用计划|
|assignedUnkownSyncState|3|Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步|
|notAssigned|4|未分配|
|挂起|5|待处理的工作分配|
|failed|6| 工作分配失败|





