---
title: meetingCapability 资源类型
description: 包含会议的功能
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2b891a9e6d0eb90a527c79528e9fd595c2f8ca5b
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913623"
---
# <a name="meetingcapability-resource-type"></a>meetingCapability 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含会议的功能

## <a name="properties"></a>属性

| 属性                          | 类型    | 说明                                                        |
|:----------------------------------|:--------|:-------------------------------------------------------------------|
| allowAnonymousUsersToDialOut      | Boolean | 指示是否允许在会议中拨出匿名用户。 |
| allowAnonymousUsersToStartMeeting | Boolean | 指示是否允许匿名用户启动会议。  |
| autoAdmittedUsers                 | String  | 可取值为：`everyoneInCompany`、`everyone`。              |

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
