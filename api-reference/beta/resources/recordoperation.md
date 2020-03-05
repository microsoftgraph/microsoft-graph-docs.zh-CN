---
title: recordOperation 资源类型
description: 包含与音频录音相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f34d3367b104ca5c1645ce3d4c95b184dcb6009
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521220"
---
# <a name="recordoperation-resource-type"></a>recordOperation 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与音频录音相关的信息。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 唯一的客户端上下文字符串。 最大限制为256个字符。                                                                                                                               |
| completionReason               | String                      | 可取值为：`operationCanceled`、`stopToneDetected`、`maxRecordDurationReached`、`initialSilenceTimeout`、`maxSilenceTimeout`、`playPromptFailed`、`playBeepFailed`、`mediaReceiveTimeout`、`unspecifiedError`、`none`。 |
| id                             | String                      | 服务器操作 ID。 只读。                                                                                              |
| recordingAccessToken           | String                      | 检索录制所需的访问令牌。                                                                                              |
| recordingLocation              | String                      | 录制所在的位置。                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                              |
| status                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordOperation"
}-->
```json
{
  "clientContext": "String",
  "completionReason": "operationCanceled | stopToneDetected | maxRecordDurationReached | initialSilenceTimeout | maxSilenceTimeout | playPromptFailed | playBeepFailed | mediaReceiveTimeout | unspecifiedError | none",
  "id": "String (identifier)",
  "recordingAccessToken": "String",
  "recordingLocation": "String",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "recordOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
