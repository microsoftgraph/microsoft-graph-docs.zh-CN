---
title: recordingInfo 资源类型
description: 表示参与者的录制信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962539"
---
# <a name="recordinginfo-resource-type"></a>recordingInfo 资源类型

命名空间：microsoft.graph

表示参与者的录制信息。

## <a name="properties"></a>属性

| 属性        | 类型    | 说明|
|:----------------|:--------|:----------|
| initiator     | [identitySet](identitySet.md) | 录制发起人的标识。 |
| recordingStatus | String | 可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
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
