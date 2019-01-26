---
title: commsOperation 资源类型
description: 某些长时间运行操作的状态。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 5a82020741033f81d5a4394f2e32b3f0f76a6e03
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29575644"
---
# <a name="commsoperation-resource-type"></a>commsOperation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

某些长时间运行操作的状态。

## <a name="methods"></a>方法
无

## <a name="properties"></a>属性

| 属性           | 类型                        | 说明                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| clientContext      | String                      | 客户端上下文。                                                             |
| createdDateTime    | DateTimeOffset              | 操作的开始时间。                                                |
| id                 | 字符串 （标识符）         | 操作 ID。只读。 由服务器生成。                                  |
| lastActionDateTime | DateTimeOffset              | 操作的上次活动时间。                                   |
| errorInfo          | [resultInfo](resultinfo.md) | 结果信息。 只读。 由服务器生成。                            |
| status             | operationStatus             | 可取值为 `notStarted`、`running`、`completed`、`failed`。 只读。 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "errorInfo": { "@odata.type": "microsoft.graph.resultInfo" },
  "status": "operationStatus"
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
    "@odata.type": "microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/commsoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
