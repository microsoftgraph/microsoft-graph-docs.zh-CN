---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce5fc93bfd48d4beaccac1552573c228f1e6f09
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725440"
---
# <a name="managementstate-enum-type"></a>managementState 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Microsoft Intune 中设备的管理状态。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|managed|0|设备正在管理中|
|retirePending|1|设备和 unenrolling 从管理中的过程中发生停用命令|
|retireFailed|双面|设备上的停用命令失败|
|wipePending|第三章|设备和 unenrolling 中的 "擦除" 命令在管理过程中发生|
|wipeFailed|4 |设备上的擦除命令失败|
|正常|5 |设备运行不正常。|
|deletePending|6 |在设备上发生删除命令 |
|retireIssued|7 |为设备发出了停用命令|
|wipeIssued|8 |已为设备发出擦除命令|
|wipeCanceled|9 |已取消此设备的擦除命令|
|retireCanceled|10  |已取消此设备的停用命令|
|探索|11x17|设备已被发现，但未完全注册。|





