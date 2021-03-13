---
title: connectedOrganizationMembers 复杂类型
description: connectedOrganizationMembers 类型标识租户中将允许其成为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 725926bc39583bda653294f0cc917ea7d2f08a45
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761812"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在访问包分配策略 [的请求设置中使用](accesspackageassignmentpolicy.md)。 值指示此类型标识用户的集合，即与已连接组织关联的用户，将允许这些用户 `@odata.type` `#microsoft.graph.connectedOrganizationMembers` 请求访问包。 [](connectedorganization.md)

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |String | 权利管理中连接的组织的 ID。 |
| 说明 |String | 已连接组织的名称。 只读。 |
| isBackup | 布尔 | 目前未使用。 |

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
  "id": "string (identifier)",
  "description": "string",
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


