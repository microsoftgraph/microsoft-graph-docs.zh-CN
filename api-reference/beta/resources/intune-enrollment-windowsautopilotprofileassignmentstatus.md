---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a3dfeff181fd7d6e8c2bc112f51c6f8096744eb688faaceda6bc4c4010fe99c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54139374"
---
# <a name="windowsautopilotprofileassignmentstatus-enum-type"></a>windowsAutopilotProfileAssignmentStatus 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|unknown|0|未知分配状态|
|assignedInSync|1 |在 Intune 中成功分配，并Windows自动试点计划同步|
|assignedOutOfSync|2 |在 Intune 中成功分配，与自动Windows计划不同步|
|assignedUnkownSyncState|3 |在 Intune 中成功分配，与自动试点计划同步Windows不同步|
|notAssigned|4 |未分配|
|pending|5 |挂起的工作分配|
|failed|6 | 分配失败|




