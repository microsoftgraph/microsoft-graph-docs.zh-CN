---
title: meetingParticipantInfo 资源类型
description: 有关会议参与者的信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 505a31673ea110f899b37b7d6404b5020ed6d88e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59113649"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

有关会议参与者的信息。

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| identity | [identitySet](identityset.md) | 参与者的身份信息。                                            |
| upn      | String                        | 参与者的用户主体名称。                                             |
| role     | onlineMeetingRole             | 指定会议参与者的角色。  可能的值为 `attendee` `presenter` 、、 `producer` 和 `unknownFutureValue` 。|

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

