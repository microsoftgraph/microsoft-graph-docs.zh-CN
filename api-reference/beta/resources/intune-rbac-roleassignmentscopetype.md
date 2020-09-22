---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 16781d47a9db63bd346c4c33efe3cbcdd278a5e3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48039515"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定角色分配的作用域的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许分配给指定的 ResourceScopes。|
|allDevices|1 |允许向所有 Intune 设备分配作业。|
|allLicensedUsers|2 |允许向所有 Intune 许可用户分配作业。|
|allDevicesAndLicensedUsers|第三章|允许分配给所有 Intune 设备和许可的用户。|






