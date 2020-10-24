---
title: meetingParticipantInfo 资源类型
description: 会议参与者的相关信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: a642532579d127fdeb48b4c69524975b293ff959
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48741997"
---
# <a name="meetingparticipantinfo-resource-type"></a>meetingParticipantInfo 资源类型

命名空间：microsoft.graph

会议参与者的相关信息。

## <a name="properties"></a>属性

| 属性 | 类型                          | 说明                                                                         |
| :------- | :---------------------------- | :---------------------------------------------------------------------------------- |
| 窃取 | [identitySet](identityset.md) | 参与者的标识信息。                                            |
| upn      | String                        | 参与者的用户主体名称。                                             |
| role     | onlineMeetingRole             | 指定参与者在会议中的角色。  下表中列出了可能的值。 |

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

