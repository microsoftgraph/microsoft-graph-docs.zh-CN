---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 62ce735d5719ef05c5f96de546adcd5518a72786
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521227"
---
# <a name="recordinginfo-resource-type"></a>recordingInfo 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

记录参与者的信息。

## <a name="properties"></a>属性

| 属性        | 类型    | 说明|
|:----------------|:--------|:----------|
| initiatedBy     | [participantInfo](participantinfo.md) | 启动录制的参与者。 |
| recordingStatus | String | 可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。 |
| initiator | [identitySet](identitySet.md) | 记录发起方的标识。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
