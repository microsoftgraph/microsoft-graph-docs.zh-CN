---
title: inviteParticipantsOperation 资源类型
description: 表示长时间运行的参与者邀请操作的状态，由对参与者邀请 API 的调用触发。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 24fb78d2c2dee1bcf902849f10eaf3d11a167426
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084389"
---
# <a name="inviteparticipantsoperation-resource-type"></a>inviteParticipantsOperation 资源类型

命名空间：microsoft.graph

表示长时间运行的参与者邀请操作的状态，由对参与者邀请 API 的调用触发。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| clientContext                  | String                      | 客户端上下文。                                                                                                                               |
| id                             | String                      | 服务器操作 ID。只读。                                                                                              |
| participants | [invitationParticipantInfo](invitationParticipantInfo.md) 集合 | 要邀请的参与者。 |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                             |
| status                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                  |

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

