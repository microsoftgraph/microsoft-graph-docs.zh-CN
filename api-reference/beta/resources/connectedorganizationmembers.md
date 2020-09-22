---
title: connectedOrganizationMembers 复杂类型
description: ConnectedOrganizationMembers 类型标识租户中将允许作为请求者、审批者或审阅者的用户的集合。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d2df6b91ebcbc65f03ee39103768bdfad04df62f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48027193"
---
# <a name="connectedorganizationmembers-complex-type"></a>connectedOrganizationMembers 复杂类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在 [访问包分配策略](accesspackageassignmentpolicy.md)的请求设置中使用。 `@odata.type`该值 `#microsoft.graph.connectedOrganizationMembers` 指示此类型标识用户的集合，这些用户与[已连接的组织](connectedorganization.md)相关联，将允许其请求访问包。

## <a name="properties"></a>属性

此类型具有以下属性：

| 属性                     | 类型                      | 说明 |
| :--------------------------- | :------------------------ | :---------- |
| id |String | 在 "权限管理" 中连接的组织的 ID。 |
| description |String | 连接的组织的名称。 只读。 |
| isBackup | Boolean | 目前未使用。 |

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


