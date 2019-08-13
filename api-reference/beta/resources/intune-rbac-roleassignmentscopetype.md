---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6699af01c2e2a2e03e0d5ef00cce0fb572d8c57d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369239"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定角色分配的作用域的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许分配给指定的 ResourceScopes。|
|allDevices|1|允许向所有 Intune 设备分配作业。|
|allLicensedUsers|双面|允许向所有 Intune 许可用户分配作业。|
|allDevicesAndLicensedUsers|第三章|允许分配给所有 Intune 设备和许可的用户。|



