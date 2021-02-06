---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133635"
---
# <a name="delegatedpermissionclassification-resource-type"></a>delegatedPermissionClassification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于指定委派权限的分类。

委派权限分类可以与用户同意设置结合使用，以选择允许用户同意的权限。 请参阅 ["配置最终用户如何同意应用程序以](/azure/active-directory/manage-apps/configure-user-consent) 了解有关权限分类更多信息"。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | 字符串 | **delegatedPermissionClassification 项的唯一** 标识符。 不可为 null。 只读。 |
| classification | permissionClassificationType | 给定的分类值。 可能的值： `low` . 不支持 `$filter`。 |
| permissionId | Guid | [servicePrincipal](servicePrincipal.md) **() 的 publishedPermissionScopes** 集合中列出的委派权限的唯一标识符 id。  创建时为必需项。 不支持 `$filter`。 |
| permissionName | 字符串 | the claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md). 不支持 `$filter`。 |

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

