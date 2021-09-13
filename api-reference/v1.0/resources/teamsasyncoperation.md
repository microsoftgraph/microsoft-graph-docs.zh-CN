---
title: teamsAsyncOperation 资源类型
description: '异步Microsoft Teams操作将超出单个 API 请求的生存期。 '
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a061ba8951013c12e825141f5a205c3e6d664733
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59071894"
---
# <a name="teamsasyncoperation-resource-type"></a>teamsAsyncOperation 资源类型

命名空间：microsoft.graph



a Microsoft Teams async operation is an operation that lifetimes the lifetime of a single API request. 这些操作长时间运行或成本过高，在发起请求的时间范围内无法完成。

启动异步操作时，该方法返回 202 Accepted 响应代码。 响应还将包含 Location 标头，其中包含 teamsAsyncOperation 的位置。 通过对此位置提出 GET 请求来定期检查操作的状态;检查>等待 30 秒。
当请求成功完成时，状态将为"已成功"，targetResourceLocation 将指向已创建/已修改的资源。

## <a name="properties"></a>属性

| 属性 | 类型   | 说明 |
|:---------------|:--------|:----------|
|id|string |唯一操作 ID。|
|operationType|[teamsAsyncOperationType](teamsasyncoperationtype.md) |表示正在描述的操作类型。|
|createdDateTime|DateTimeOffset |创建操作的时间。|
|status|[teamsAsyncOperationStatus](teamsasyncoperationstatus.md)| 操作状态。|
|lastActionDateTime|DateTimeOffset |上次更新异步操作的时间。|
|attemptsCount|Int32|在标记为成功或失败之前尝试该操作次数。|
|targetResourceId|guid |由于此异步操作而创建或修改的对象（通常为团队）的[ID。](../resources/team.md)|
|targetResourceLocation|string|由于此异步操作而创建或修改的对象的位置。 此 URL 应视为不透明值，而不是解析到其组件路径。|
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

