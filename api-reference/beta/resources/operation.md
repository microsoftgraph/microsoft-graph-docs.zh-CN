---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
ms.openlocfilehash: e1e0f7a886d460bc378fdc75041e17b997897e2d
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341769"
---
# <a name="operation-resource-type"></a>操作资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

长时间运行的操作的状态。

## <a name="methods"></a>方法

无

## <a name="properties"></a>属性

| 属性           | 类型            | 说明                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | 操作的开始时间。                                                |
| id                 | String          | 操作 id。只读。 由服务器生成。                                  |
| lastActionDateTime | DateTimeOffset  | 操作的上一操作的时间。                                   |
| status             | String          | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>关系

无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>示例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.operation"
}-->
```json
{
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "status": "completed"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
