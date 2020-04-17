---
title: recordingInfo 资源类型
description: 表示参与者的录制信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543266"
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
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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
