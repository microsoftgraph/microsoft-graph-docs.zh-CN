---
title: managementState 枚举类型
description: Microsoft Intune 中设备的管理状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fd0a4616f6f35c91ae6ce6269d452a00d3275bc5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783926"
---
# <a name="managementstate-enum-type"></a>managementState 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

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
|retireCanceled|10 |已取消此设备的停用命令|
|探索|11x17|设备已被发现，但未完全注册。|



