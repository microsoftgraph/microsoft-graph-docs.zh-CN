---
title: windowsAutopilotProfileAssignmentStatus 枚举类型
description: 尚未记录
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 724da31643ccc971d405c224e309bd11d49f8334
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59054245"
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
|assignedUnkownSyncState|3|在 Intune 中成功分配，与自动试点计划同步Windows不同步|
|notAssigned|4 |未分配|
|pending|5 |挂起的工作分配|
|failed|6 | 分配失败|



