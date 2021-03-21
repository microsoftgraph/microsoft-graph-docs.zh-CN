---
title: meetingCapability 资源类型
description: 包含会议功能
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d8e1d3985f95ecc28bd986218d7ff668f65b1db8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960402"
---
# <a name="meetingcapability-resource-type"></a>meetingCapability 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含会议功能

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Boolean | 指示是否允许在会议中匿名用户拨出。 |
| allowAnonymousUsersToStartMeeting | Boolean | 指示是否允许匿名用户启动会议。  |
| autoAdmittedUsers                 | autoAdmittedUsersType  | 可取值为：`everyoneInCompany`、`everyone`。              |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingCapability"
}-->
```json
{
  "allowAnonymousUsersToDialOut": true,
  "allowAnonymousUsersToStartMeeting": true,
  "autoAdmittedUsers": "everyoneInCompany | everyone"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingCapability resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


