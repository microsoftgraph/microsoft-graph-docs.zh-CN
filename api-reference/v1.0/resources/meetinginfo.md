---
title: meetingInfo 资源类型
description: 为创建或加入会议而指定的会议信息。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0df2c90c8600fea2b00cf465c17682714b0c8a6e
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59134589"
---
# <a name="meetinginfo-resource-type"></a>meetingInfo 资源类型

命名空间：microsoft.graph

这是包含会议特定信息的抽象类。
 
若要加入现有会议，必须将 [organizerMeetingInfo](organizermeetinginfo.md) 与 [chatInfo](./chatinfo.md)结合使用，或仅指定 [tokenMeetingInfo](tokenmeetinginfo.md)。


## <a name="derived-types"></a>派生类型

| 类型                                                 | 说明                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [organizerMeetingInfo](./organizermeetinginfo.md)    | 有关会议组织者的详细信息                          |
| [tokenMeetingInfo](tokenmeetinginfo.md)              | 包含有关会议信息的加密令牌  |

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

