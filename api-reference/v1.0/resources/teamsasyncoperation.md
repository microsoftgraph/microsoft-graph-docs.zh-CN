---
title: teamsAsyncOperation 资源类型
description: 'Microsoft 团队异步操作 transcends 单个 API 请求的生存期。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c11527f5a05018f02b4f3113ffa52e10e8929cfd
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078967"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation 资源类型

命名空间：microsoft.graph



Microsoft 团队 async operation 是 transcends 一个 API 请求的生存期的操作。 这些操作运行时间较长，或者在发起请求的时间范围内完成的成本太高。

当异步操作启动时，该方法将返回202接受的响应代码。 该响应还将包含一个位置标头，其中包含 teamsAsyncOperation 的位置。 通过向此位置发出 GET 请求来定期检查操作的状态;在两个检查之间等待 >30 秒。
当请求成功完成时，状态将为 "已成功"，targetResourceLocation 将指向 "已创建/已修改" 的资源。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|id|string |唯一操作 id。|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |指示正在描述的操作的类型。|
|createdDateTime|DateTimeOffset |创建操作的时间。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作状态。|
|lastActionDateTime|DateTimeOffset |上次更新异步操作的时间。|
|attemptsCount|Int32|在标记为 "成功" 或 "失败" 之前尝试操作的次数。|
|targetResourceId|containerparentjob |作为此异步操作（通常为 [团队](../resources/team.md)）的结果创建或修改的对象的 ID。|
|targetResourceLocation|string|作为此异步操作的结果创建或修改的对象的位置。 应将此 URL 视为不透明值，而不会将其解析为其组件路径。|
|error|[operationError](operationerror.md)|导致异步操作失败的任何错误。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.teamsAsyncOperation"
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
<!-- {
  "type": "#page.annotation",
  "description": "teams async operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

