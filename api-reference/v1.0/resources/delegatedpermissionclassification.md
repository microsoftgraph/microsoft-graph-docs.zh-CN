---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff9f4ca394e2065c69fd7cd08a19d60817fc4f99
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761756"
---
# <a name="delegatedpermissionclassification-resource-type"></a>delegatedPermissionClassification 资源类型

命名空间：microsoft.graph

用于指定委派权限的分类。

委派权限分类可以与用户同意设置结合使用，以选择允许用户同意的权限。 [请参阅配置最终用户如何同意应用程序](/azure/active-directory/manage-apps/configure-user-consent)以了解有关权限分类有关详细信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | 字符串 | **delegatedPermissionClassification 项的唯一** 标识符。 不可为 null。 只读。 |
| classification | permissionClassificationType | 给定的分类值。 可能的值 `low` ：。 不支持 `$filter`。 |
| permissionId | Guid | [servicePrincipal](servicePrincipal.md) ( **oauth2PermissionScopes** 集合) 委派权限的唯一标识符 id。 创建时为必需项。 不支持 `$filter`。 |
| permissionName | 字符串 | 声明值 ([servicePrincipal](servicePrincipal.md)) **oauth2PermissionScopes** 集合中列出的委派权限的值。  不支持 `$filter`。 |

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
