---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d0198ae992dc3e741c2962ed4e2c9534f5a76757
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865780"
---
# <a name="inviteparticipantsoperation-resource-type"></a>inviteParticipantsOperation 资源类型

表示长时间运行的参与者邀请操作的状态，通过调用参与者-邀请 API 触发。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 客户端上下文。                                                                                                                               |
| id                             | String                      | 服务器操作 id。只读。                                                                                              |
| participants | [invitationParticipantInfo](invitationParticipantInfo.md) 集合 | 要邀请的参与者。 |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                             |
| 状态                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                  |

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
  "id": "String (identifier)",
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
