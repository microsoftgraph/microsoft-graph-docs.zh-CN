---
title: entitlementManagementSettings 资源类型
description: 表示用于授权管理的租户Azure AD设置。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d578781ed4b9b03d9a375a7cd9875df2f6fc4d0f
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649762"
---
# <a name="entitlementmanagementsettings-resource-type"></a>entitlementManagementSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示控制授权管理[Azure AD的设置](entitlementmanagement-overview.md)。  此资源不包括目录创建者设置;若要查看或更改目录创建者角色成员身份，请使用角色 [分配](unifiedroleassignment.md) API 和权利管理 RBAC 提供程序。

## <a name="methods"></a>方法

| 方法       | 返回类型 | 说明 |
|:-------------|:------------|:------------|
| [获取](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 读取 **entitlementManagementSettings 对象** 的属性。 |
| [更新](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | 更新 **entitlementManagementSettings 对象** 的属性。 |

## <a name="properties"></a>属性

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|String|、 `None` `BlockSignIn` 或 `BlockSignInAndDelete` 之一。 |
|daysUntilExternalUserDeletedAfterBlocked|Int64|如果 **externalUserLifecycleAction** 为 ，则外部用户在删除其帐户之前被阻止 `BlockSignInAndDelete` 登录的天数。|

## <a name="relationships"></a>关系

无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


