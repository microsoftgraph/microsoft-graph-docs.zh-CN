---
title: recordOperation 资源类型
description: 此资源类型包含与音频录音相关的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b4f0a62204a6ee1db7e75caf9044288f705a5529
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865768"
---
# <a name="recordoperation-resource-type"></a>recordOperation 资源类型

此资源类型包含与音频录音相关的信息。

## <a name="properties"></a>属性

| 属性                       | 类型                        | 说明                                                                                                                                       |
| :----------------------------- | :---------------------------| :-------------------------------------------------------------------------------------------------------------------------------------------------|
| 适用                  | String                      | 唯一的客户端上下文字符串。 最大限制为256个字符。                                                                                                                               |
| id                             | String                      | 服务器操作 id。只读。                                                                                              |
| recordingAccessToken           | String                      | 检索录制所需的访问令牌。                                                                                              |
| recordingLocation              | String                      | 录制所在的位置。                                                                                                      |
| resultInfo                     | [resultInfo](resultinfo.md) | 结果信息。  只读。                                                                                              |
| 状态                         | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。 只读。                                                |

## <a name="relationships"></a>关系
无

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
