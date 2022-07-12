---
title: meetingInfo 资源类型
description: 指定用于创建或加入会议的会议信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d7aebdbd0236f0c1223e295456d408f37fb0708e
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2022
ms.locfileid: "66731587"
---
# <a name="meetinginfo-resource-type"></a>meetingInfo 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

这是一个抽象类，包含特定于会议的信息。
 
若要加入现有会议，必须将 [organizerMeetingInfo](organizermeetinginfo.md) 与 [chatInfo](./chatinfo.md)、 [tokenMeetingInfo](tokenmeetinginfo.md) 或 [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md) 结合指定。


## <a name="derived-types"></a>派生类型

| 类型                                                    | 说明                                                         |
|:--------------------------------------------------------|:--------------------------------------------------------------------|
| [joinMeetingIdMeetingInfo](joinmeetingidmeetinginfo.md) | 包含会议的 **joinMeetingId** 和 **密码** 。     |
| [organizerMeetingInfo](./organizermeetinginfo.md)       | 有关会议组织者的详细信息。                         |
| [tokenMeetingInfo](tokenmeetinginfo.md)                 | 包含有关会议信息的加密令牌。 |

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


