---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68612e2f4ccee46612c82237630efafda484b7e9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419119"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知的工作分配状态|
|assignedInSync|1|分配 Intune 中成功的 Windows 自动试用计划同步|
|assignedOutOfSync|2|分配 Intune 中成功的不与同步 Windows 自动试用计划|
|assignedUnkownSyncState|3|Intune 和任一中同步中成功分配或与 Windows 自动试用计划不同步|
|notAssigned|4|未分配|
|挂起|5|待处理的工作分配|
|failed|6| 工作分配失败|




