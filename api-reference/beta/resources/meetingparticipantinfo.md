---
title: meetingParticipantInfo 资源类型
description: 有关会议参与者的信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5d3f8e5fb055fa45ef150aa9ef7eef82980d0755
ms.sourcegitcommit: 0e7927f34b7e55d323acbf281e11560cb40a89ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2022
ms.locfileid: "63668582"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议参与者的信息。

## <a name="properties"></a>属性

| 属性 | 类型             | 说明                 |
| :------- | :-------------------- | :------------------------------ |
| identity | [identitySet](identityset.md) | 参与者的身份信息。           |
| upn      | String                        | 参与者的用户主体名称。             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | 指定会议参与者的角色。|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

下表列出了可发展枚举 [的成员](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)。 必须使用请求标头 `Prefer: include-unknown-enum-members` 获取此 `coorganizer` 可发展枚举中的值。

| 值              | 说明                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | 参与者的角色为与会者。 此值适用于所有会议。   |
| 演示者           | 参与者的角色是演示者。 此值适用于 **allowedPresenter** `roleIsPresenter`设置为 或 Teams实时事件的会议。 |
| producer            | 参与者的角色是制作者。 此值仅适用于Teams事件。  |
| coorganizer | 参与者的角色是共同组织者。 此值适用于除实时事件Teams会议。 |
| unknownFutureValue | 可发展枚举 sentinel 值。 请勿使用。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String",
  "role": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


