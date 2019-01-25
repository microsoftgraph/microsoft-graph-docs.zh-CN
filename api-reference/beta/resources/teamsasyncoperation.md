---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 61c26b0d594ccdbad8020557f60c6f6b23a83254
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513457"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Microsoft 团队异步操作是超越单个 API 请求的生命周期的操作。 这些操作是运行时间较长或太高完成其原始请求的时间范围。

启动异步操作后，该方法将返回 202 接受响应代码。 响应还将包含位置标头，其中包含 teamsAsyncOperation 的位置。 定期检查通过对此位置; 进行 GET 请求的操作的状态等待 >30 之间检查的秒数。
请求成功完成时，状态将为"成功"，并且 targetResourceLocation 将指向创建修改资源。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|id|string |唯一的操作的 id。|
|： 键入|[teamsAsyncOperationType](teamsasyncoperationtype.md) |表示所描述的操作的类型。|
|createdDateTime|DateTimeOffset |创建操作的时间。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作状态。|
|lastActionDateTime|DateTimeOffset |上次更新时间异步操作的时间。|
|attemptsCount|Int32|操作已被标记为成功或失败前尝试次数。|
|targetResourceId|Guid |创建或修改此异步操作，通常[团队](../resources/team.md)的结果的对象 ID。|
|targetResourceLocation|string|对象已创建或修改此异步操作的结果的位置。 此 URL 应视为不透明的值，并不解析到它的组件路径。|
|error|[operationError](operationerror.md)|使异步操作失败的任何错误。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsasyncoperation"
}-->

```json
{
    "id": "string",
    "operationType": "archiveTeam",
    "createdDateTime": "2018-01-01T00:00:00.0000000Z",
    "status": "succeeded",
    "lastActionDateTime": "2018-01-01T00:00:00.0000000Z",
    "attemptsCount": 1,
    "targetResourceId": "fa4aa5a2-a75b-4769-86f4-9e2742a18fda",
    "targetResourceLocation": "/groups('fa4aa5a2-a75b-4769-86f4-9e2742a18fda')/team",
    "error": null
}
```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
