---
title: meetingParticipantInfo 资源类型
description: 有关会议参与者的信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2222c32db1f4dcee27fb4e3c88100d5e32788f60
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883864"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议参与者的信息。

## <a name="properties"></a>属性

| 属性 | 类型             | 说明                 |
| :------- | :-------------------- | :------------------------------ |
| 身份 | [identitySet](identityset.md) | 参与者的标识信息。           |
| Upn      | String                        | 参与者的用户主体名称。             |
| role     | [onlineMeetingRole](#onlinemeetingrole-values)     | 指定参与者在会议中的角色。|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

下表列出了 [可旋转枚举](/graph/best-practices-concept#handling-future-members-in-evolvable-enumerations)的成员。 必须使用 `Prefer: include-unknown-enum-members` 请求标头获取 `coorganizer` 此可旋转枚举中的值。

| 值              | 说明                                                            |
| ------------------ | ---------------------------------------------------------------------- |
| attendee            | 参与者的角色是与会者。 此值适用于所有会议。   |
| 主持人           | 参与者的角色是演示者。 此值适用于已设置为 `roleIsPresenter`**allowedPresenter** 的会议或 Teams 实时事件。 |
| 生产者            | 参与者的角色是生成者。 此值仅适用于 Teams 实时事件。  |
| coorganizer | 参与者的角色是共同组织者。 此值适用于除 Teams 直播活动以外的所有会议。 |
| unknownFutureValue | 可变枚举 sentinel 值。 请勿使用。 |

> [!TIP]
>
> 若要在创建或更新 [OnlineMeeting](onlinemeeting.md) 时设置会议与会者的 **演示** 者角色，还必须将 **allowedPresenters** 的值设置为 `roleIsPresenter`。

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


