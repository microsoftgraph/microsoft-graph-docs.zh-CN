---
title: updateRecordingStatusOperation 资源类型
description: 描述更新录制状态操作的响应格式。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1f377ac39ec8e216b883f644f086f888b025ef8c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59062409"
---
# <a name="updaterecordingstatusoperation-resource-type"></a>updateRecordingStatusOperation 资源类型

命名空间：microsoft.graph

描述更新录制状态操作的响应格式。

## <a name="properties"></a>属性

| 属性            | 类型                        | 说明|
|:--------------------|:----------------------------|:-----------------------------------------------------------------------------------|
| clientContext       | String                      | 唯一的客户端上下文字符串。 最大限制为 256 个字符。                              |
| id                  | String                      | 只读。                                                                         |
| resultInfo          | [resultInfo](resultinfo.md) | 结果信息。 只读。                                                 |
| status              | String                      | 可能的值是：`notStarted`、`running`、`completed`、`failed`。               |

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.updateRecordingStatusOperation"
}-->
```json
{
  "clientContext": "String",
  "id": "String (identifier)",
  "resultInfo": {"@odata.type": "#microsoft.graph.resultInfo"},
  "status": "notStarted | running | completed | failed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "updateRecordingStatusOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

