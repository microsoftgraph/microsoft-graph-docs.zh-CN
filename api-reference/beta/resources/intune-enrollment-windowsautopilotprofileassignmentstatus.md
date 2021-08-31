---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: addd0a3ab96c75cc62d380f16a0b82006870cdfa
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58788925"
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
|assignedInSync|1|在 Intune 中成功分配，并Windows自动试点计划同步|
|assignedOutOfSync|2|在 Intune 中成功分配，与自动Windows计划不同步|
|assignedUnkownSyncState|3|在 Intune 中成功分配，与自动试点计划同步或Windows同步|
|notAssigned|4 |未分配|
|pending|5 |挂起的工作分配|
|failed|6 | 分配失败|



