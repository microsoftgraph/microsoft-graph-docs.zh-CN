---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: a974bd22ddd9e1ac8c6ab90cdedb9dda9f1a1bb5
ms.sourcegitcommit: c68a83d28fa4bfca6e0618467934813a9ae17b12
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/07/2019
ms.locfileid: "36793021"
---
# <a name="inviteparticipantsoperation-resource-type"></a>inviteParticipantsOperation 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 客户端上下文。                                                                                                                               |
| createdDateTime                | DateTimeOffset              | 创建录制的时间。                                                                                                          |
| id                             | String                      | 服务器操作 id。只读。 由服务器生成。                                                                                             |
| lastActionDateTime             | DateTimeOffset              | 操作的上一操作的时间。                                                                                                     |
| participants | [invitationParticipantInfo](invitationParticipantInfo.md)集合 | 要邀请的参与者。 |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。 由服务器生成。                                                                                             |
| status                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。 由服务器生成。                                                 |

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inviteParticipantsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "participants": [{"@odata.type": "#microsoft.graph.invitationParticipantInfo"}],
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inviteParticipantsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
