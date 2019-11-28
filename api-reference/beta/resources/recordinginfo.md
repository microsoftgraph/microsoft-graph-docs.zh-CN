---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: d9e9a17a9afb197333e677547f3fa5dca22df9b2
ms.sourcegitcommit: fce7ce328f0c88c6310af9cc85d12bcebc88a6c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/28/2019
ms.locfileid: "39637043"
---
# <a name="recordinginfo-resource-type"></a>recordingInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

记录参与者的信息。

## <a name="properties"></a>属性

| 属性        | 类型    | 说明|
|:----------------|:--------|:----------|
| initiatedBy     | [participantInfo](participantinfo.md) | 启动录制的参与者。 |
| recordingStatus | String | 可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。 |

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
