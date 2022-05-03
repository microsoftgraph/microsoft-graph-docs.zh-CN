---
title: 操作资源类型
description: 长时间运行的操作的状态。
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: teamwork
author: billbliss
ms.openlocfilehash: c1f07f81754b1cf0373917bbb59953fd1342d627
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176515"
---
# <a name="operation-resource-type"></a>操作资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

长时间运行的操作的状态。

## <a name="methods"></a>方法

无。

## <a name="properties"></a>属性

| 属性           | 类型            | 说明                                                                     |
| :----------------- | :-------------- | :-------------------------------------------------------------------------------|
| createdDateTime    | DateTimeOffset  | 操作的开始时间。                                                |
| id                 | String          | 操作 ID。 只读。 由服务器生成。                                  |
| lastActionDateTime | DateTimeOffset  | 操作的最后一个操作的时间。                                   |
| 状态             | String          | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>关系

无。

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


