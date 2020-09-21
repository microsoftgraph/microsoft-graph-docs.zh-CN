---
title: plannerUserIds 资源类型
description: '**PlannerUserIds**资源表示与计划共享的用户 id 的列表。 这是开放类型。 如果您利用的是 Microsoft 365 组，请使用组 API 来管理组成员身份，以共享组的计划。 您还可以将组的现有成员添加到此集合中，但它们不需要他们访问该组拥有的计划。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b2fec8b10079047b6020114197bc5f68f25298d0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063967"
---
# <a name="planneruserids-resource-type"></a>plannerUserIds 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**PlannerUserIds**资源表示与[计划](plannerplan.md)共享的用户 id 的列表。 这是开放类型。 如果您利用的是 Microsoft 365 组，请使用组 API 来管理组成员身份，以共享 [组的](group.md) 计划。 您还可以将组的现有成员添加到此集合中，但它们不需要他们访问该组拥有的计划。


## <a name="properties"></a>属性
可由客户端定义打开类型的属性。 在这种情况下，客户端应将用户 id 作为属性提供，其值为 `true` boolean。 当不再与用户 id 共享时，将通过将属性值设置为布尔值来自动删除属性 `false` 。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerUserIds"
}-->

```json
{
  "String-value": true
}
```

### <a name="example"></a>示例
```json
{
  "400723e1-102b-43aa-aba9-f35524827084": true, // property name is user id
  "f117339e-c914-4a9c-9b66-1c062b027556": true,
  "e886d105-23b9-47e2-bde1-757e75ee4a28": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


