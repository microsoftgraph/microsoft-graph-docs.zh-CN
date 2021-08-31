---
title: roleAssignmentScopeType 枚举类型
description: 指定角色分配的范围类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3de3f4852b25228e35aa5834fe8e984c6de953bc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802941"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 枚举类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定角色分配的范围类型。

## <a name="members"></a>成员
|成员|值|说明|
|:---|:---|:---|
|resourceScope|0|允许将工作分配指定 ResourceScopes。|
|allDevices|1|允许分配至所有 Intune 设备。|
|allLicensedUsers|2|允许分配给所有 Intune 许可用户。|
|allDevicesAndLicensedUsers|3|允许分配至所有 Intune 设备和许可用户。|



