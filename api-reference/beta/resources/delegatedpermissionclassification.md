---
title: delegatedPermissionClassification 资源类型
description: 用于指定委派权限的分类。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 72cc4630ba8f28fe0d76722178edcdd3ffed5943
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854641"
---
# <a name="delegatedpermissionclassification-resource-type"></a>delegatedPermissionClassification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于指定委派权限的分类。

委派权限分类可以与用户同意设置结合使用，以选择允许用户同意的权限。 [请参阅配置最终用户如何同意应用程序以](/azure/active-directory/manage-apps/configure-user-consent)了解有关权限分类有关详细信息。

## <a name="properties"></a>属性

| 属性 | 类型 | 说明 |
|:---------------|:--------|:----------|
| id | String | **delegatedPermissionClassification 项的唯一** 标识符。 不可为 null。 只读。 |
| classification | permissionClassificationType | 给定的分类值。 可能的值： `low`。 不支持 `$filter`。 |
| permissionId | GUID | [servicePrincipal](servicePrincipal.md) (**publishedPermissionScopes** 集合) 委派权限的唯一标识符 id。 创建时为必需项。 不支持 `$filter`。 |
| permissionName | String | 声明值 ([servicePrincipal](servicePrincipal.md)) **publishedPermissionScopes** 集合中列出的委派权限。 不支持 `$filter`。 |

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

