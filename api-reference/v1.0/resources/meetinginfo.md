---
title: meetingInfo 资源类型
description: 指定用于创建或加入会议的会议信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e777de1b9f6710156106ce8dab5704613b98e1e5
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871073"
---
# <a name="meetinginfo-resource-type"></a>meetingInfo 资源类型

这是一个包含会议特定信息的抽象类。
 
若要加入现有会议，必须将[organizerMeetingInfo](organizermeetinginfo.md)与[chatInfo](./chatinfo.md)或仅指定[tokenMeetingInfo](tokenmeetinginfo.md)一起指定。


## <a name="derived-types"></a>派生类型

| 类型                                                 | 说明                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [organizerMeetingInfo](./organizermeetinginfo.md)    | 有关会议组织者的详细信息                          |
| [tokenMeetingInfo](tokenmeetinginfo.md)              | 包含有关会议的信息的加密令牌  |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
