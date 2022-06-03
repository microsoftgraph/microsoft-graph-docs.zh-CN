---
title: meetingParticipantInfo 资源类型
description: 有关会议参与者的信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d46f15a86742a23b6ec4e9f6c270308de34c169c
ms.sourcegitcommit: 9adff6756e27aabbf36a9adbc2269b13c7fa74ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/03/2022
ms.locfileid: "65883983"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

有关会议参与者的信息。

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| 身份 | [identitySet](identityset.md) | 参与者的标识信息。                                            |
| Upn      | String                        | 参与者的用户主体名称。                                             |
| role     | onlineMeetingRole             | 指定参与者在会议中的角色。  可能的值是`attendee`， `presenter`和 `producer``unknownFutureValue`.|

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

