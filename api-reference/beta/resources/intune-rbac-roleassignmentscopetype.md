---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的作用域的类型。
ms.openlocfilehash: dcfac7b345dde2d8f107b8ec756d017966a6a94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046696"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

指定角色分配的作用域的类型。
## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许分配给指定 ResourceScopes。|
|allDevices|1|允许分配给所有 Intune 设备。|
|allLicensedUsers|2|允许分配给所有 Intune 授权用户。|
|allDevicesAndLicensedUsers|3|允许分配给所有 Intune 设备和授权的用户。|





