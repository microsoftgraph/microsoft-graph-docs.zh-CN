---
title: entitlementManagementSettings 资源类型
description: 表示用于授权管理的租户Azure AD范围设置。
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3f8ce8cdbc275ab32a5a84164716226fb6d2dddf
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649695"
---
# <a name="entitlementmanagementsettings-resource-type"></a>entitlementManagementSettings 资源类型

命名空间：microsoft.graph


表示控制授权管理[Azure AD的设置](entitlementmanagement-overview.md)。 此资源不包括目录创建者设置;若要查看或更改目录创建者角色成员身份，请使用角色 [分配](unifiedroleassignment.md) API 和权利管理 RBAC 提供程序。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 entitlementManagementSettings](../api/entitlementmanagementsettings-get.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|读取 **entitlementManagementSettings 对象** 的属性。 |
|[更新 entitlementManagementSettings](../api/entitlementmanagementsettings-update.md)|[entitlementManagementSettings](entitlementmanagementsettings.md)|更新 **entitlementManagementSettings 对象** 的属性。 |

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|durationUntilExternalUserDeletedAfterBlocked|期限|如果 **externalUserLifecycleAction** 为 ，在删除外部用户的帐户之前阻止其登录的持续时间（通常为 `blockSignInAndDelete` 几天）。|
|externalUserLifecycleAction|accessPackageExternalUserLifecycleAction|删除外部用户的最后一个访问包分配时该服务应执行自动操作。 可能的值包括 `none`、`blockSignIn`、`blockSignInAndDelete`、`unknownFutureValue`。|
|id|String|常量。 只读。|

## <a name="relationships"></a>关系
无。
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.entitlementManagementSettings",
  "id": "String",
  "externalUserLifecycleAction": "String",
  "durationUntilExternalUserDeletedAfterBlocked": "String (duration)"
}
```

