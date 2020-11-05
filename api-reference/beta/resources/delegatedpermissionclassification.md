---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f3d35c11ffe29feafed025b95c8f221e4f9ee4cb
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921730"
---
# <a name="delegatedpermissionclassification-resource-type"></a>delegatedPermissionClassification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于指定委派权限的分类。

委派权限分类可与用户同意设置结合使用，以选择允许用户同意的权限。 请参阅 [配置最终用户同意应用程序的方式](/azure/active-directory/manage-apps/configure-user-consent) ，以了解有关权限分类的详细信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | String | **DelegatedPermissionClassification** 项的唯一标识符。 不可为 null。 只读。 |
| classification | permissionClassificationType | 所提供的分类值。 可能的值： `low` 。 不支持 `$filter`。 |
| permissionId | Guid | [ServicePrincipal](servicePrincipal.md)的 **publishedPermissionScopes** 集合中列出的委派权限 ( **id** ) 唯一标识符。 创建时为必需项。 不支持 `$filter`。 |
| permissionName | String | 对于 [servicePrincipal](servicePrincipal.md)的 **publishedPermissionScopes** 集合中列出的委派权限，声明值 ( **值** ) 。 不支持 `$filter`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```
