---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8e77322dee3f8d94fe8eaee226dce029133a578d
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635192"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含有关会议参与者的信息。

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                                        |
| :------- | :---------------------------- | :--------------------------------------------------------------------------------- |
| 窃取 | [identitySet](identityset.md) | 参与者的标识信息。                                           |
| upn      | String                        | 参与者的用户主体名称。                                            |
| role     | onlineMeetingRole             | 指定参与者在会议中的角色。  可取值为：`attendee`、`presenter` 和 `unknownFutureValue`。|

### <a name="onlinemeetingrole-values"></a>onlineMeetingRole 值

| 值              | 说明                     |
| ------------------ | ------------------------------- |
| attendee           | 参与者是与会者。 |
| 演示者          | 参与者是演示者。 |
| 向 unknownfuturevalue | 未知的未来值。           |

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


