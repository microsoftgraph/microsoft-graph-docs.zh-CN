---
title: meetingInfo 资源类型
description: 为创建或加入会议而指定的会议信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab866ada9fa4b886cbd90cb999132ff13b48d74437f11710a43aee31ba7857fe
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126408"
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

