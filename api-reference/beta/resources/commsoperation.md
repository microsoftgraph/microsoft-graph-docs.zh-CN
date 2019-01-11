---
title: commsOperation 资源类型
description: 某些长时间运行操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: d70ad6535d5ae829de4b9bac3c5b9fea9b53188b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821446"
---
# <a name="commsoperation-resource-type"></a>commsOperation 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

某些长时间运行操作的状态。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性

| 属性           | 类型                        | Description                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | 字符串                      | 客户端上下文。                                                             |
| createdDateTime    | DateTimeOffset              | 操作的开始时间。                                                |
| id                 | 字符串                      | 操作 ID。只读。 生成的服务器。                                  |
| lastActionDateTime | DateTimeOffset              | 操作的上次活动时间。                                   |
| resultInfo         | [resultInfo](resultinfo.md) | 结果的信息。 此为只读属性。 生成的服务器。                            |
| status             | String                      | 可取值为 `notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>Relationships
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a>示例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
