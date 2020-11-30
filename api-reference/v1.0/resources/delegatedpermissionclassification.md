---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377238"
---
# <a name="delegatedpermissionclassification-resource-type"></a>delegatedPermissionClassification 资源类型

命名空间：microsoft.graph

用于指定委派权限的分类。

委派权限分类可与用户同意设置结合使用，以选择允许用户同意的权限。 请参阅 [配置最终用户同意应用程序的方式](/azure/active-directory/manage-apps/configure-user-consent) ，以了解有关权限分类的详细信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | 字符串 | **DelegatedPermissionClassification** 项的唯一标识符。 不可为空。 只读。 |
| classification | permissionClassificationType | 所提供的分类值。 可能的值： `low` 。 不支持 `$filter`。 |
| permissionId | Guid | [ServicePrincipal](servicePrincipal.md)的 **oauth2PermissionScopes** 集合中列出的委派权限 (**id**) 唯一标识符。 创建时为必需项。 不支持 `$filter`。 |
| permissionName | 字符串 | 对于 [servicePrincipal](servicePrincipal.md)的 **oauth2PermissionScopes** 集合中列出的委派权限，声明值 (**值**) 。 不支持 `$filter`。 |

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
