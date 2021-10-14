---
title: connectedOrganizationMembers 复杂类型
description: connectedOrganizationMembers 类型标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
ms.localizationpriority: medium
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0baaea3f8d6e917d072b8e9f5933b3388e1a0324
ms.sourcegitcommit: f4999aa6fc05f845027db01aa489f7086f9850e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2021
ms.locfileid: "60289236"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略 [的请求设置中使用](accesspackageassignmentpolicy.md)。 值指示此类型标识用户的集合，即与已连接组织关联的用户，将允许这些用户 `@odata.type` `#microsoft.graph.connectedOrganizationMembers` 请求访问包。 [](connectedorganization.md)

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |字符串 | 权利管理中连接的组织的 ID。 |
| 说明 |字符串 | 已连接组织的名称。 只读。 |
| isBackup | 布尔值 | 目前未使用。 |

## <a name="json-representation"></a>JSON 表示形式

以下是类型的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.connectedOrganizationMembers",
  "baseType": "microsoft.graph.userSet"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "isBackup": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "connectedOrganizationMembers complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


