---
title: plannerUserIds 资源类型
description: '**plannerUserIds** 资源表示共享计划的用户 ID 的列表。 这是"打开类型"。 如果你要利用Microsoft 365组，请使用组 API 管理组成员身份以共享组计划。 您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。'
ms.localizationpriority: medium
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 53b10f1f1ca921446279c294782ceb68dbf182f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021440"
---
# <a name="planneruserids-resource-type"></a>plannerUserIds 资源类型

命名空间：microsoft.graph

**plannerUserIds** 资源表示共享计划的用户 ID 的列表。 [](plannerplan.md) 这是"打开类型"。 如果你要利用Microsoft 365组，请使用组 API 管理组成员身份以[共享组计划](group.md)。 您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。


## <a name="properties"></a>属性
开放类型的属性可通过客户端定义。 在这种情况下，客户端应提供用户 ID 作为属性，其值为 `true` 布尔值。 当不再与用户 ID 共享时，会自动通过将其值设置为布尔值来删除 `false` 属性。


## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerUserIds resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

