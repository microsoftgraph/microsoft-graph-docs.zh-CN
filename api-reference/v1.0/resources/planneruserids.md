---
title: plannerUserIds 资源类型
description: '**plannerUserIds** 资源表示共享计划的用户 ID 的列表。 这是"打开类型"。 如果要利用组Microsoft 365，请使用组 API 管理组成员身份以共享组计划。 您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。'
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: b40b1681728bcebe85bab43254bb8414886ff3425d296596364992db7d5c8e7e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54223247"
---
# <a name="planneruserids-resource-type"></a>plannerUserIds 资源类型

命名空间：microsoft.graph

**plannerUserIds** 资源表示共享计划的用户 ID 的列表。 [](plannerplan.md) 这是"打开类型"。 如果你要利用Microsoft 365组，请使用组 API 管理组成员身份以[共享组计划](group.md)。 您还可以将组的现有成员添加到此集合中，尽管他们无需访问组所拥有的计划。


## <a name="properties"></a>属性
开放类型的属性可以通过客户端定义。 在这种情况下，客户端应提供用户 ID 作为属性，其值为 `true` 布尔值。 当不再与用户 ID 共享时，会自动通过将其值设置为布尔值来删除 `false` 属性。


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

