---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573051"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定角色分配的作用域的类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许分配给指定的 ResourceScopes。|
|allDevices|1|允许向所有 Intune 设备分配作业。|
|allLicensedUsers|2 |允许向所有 Intune 许可用户分配作业。|
|allDevicesAndLicensedUsers|3 |允许分配给所有 Intune 设备和许可的用户。|





