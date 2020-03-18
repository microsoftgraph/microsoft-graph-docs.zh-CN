---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: efdbc48a1363ba9d958c8bfe0dd2889478975083
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42773250"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定角色分配的作用域的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许分配给指定的 ResourceScopes。|
|allDevices|1|允许向所有 Intune 设备分配作业。|
|allLicensedUsers|双面|允许向所有 Intune 许可用户分配作业。|
|allDevicesAndLicensedUsers|第三章|允许分配给所有 Intune 设备和许可的用户。|



