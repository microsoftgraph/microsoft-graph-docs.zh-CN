---
title: rejectJoinResponse 资源类型
description: 包含拒绝尝试加入会议的参与者的响应。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c917b2c5ba0ed273af1c8e89c78b07a80d6c45fc
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2021
ms.locfileid: "53428856"
---
# <a name="rejectjoinresponse-resource-type"></a>rejectJoinResponse 资源类型

命名空间：microsoft.graph

包含拒绝尝试加入会议的参与者的响应。

这具有与拒绝使用 [reject-call](../api/call-reject.md) 方法记录传入呼叫通知的策略相同的效果。 机器人将继续接收新用户加入的参与者加入通知，直到达到其容量。

## <a name="properties"></a>属性

| 属性         | 类型                            | 说明                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| reason           | String                          | 拒绝原因。 可取值为：`None`、`Busy` 和 `Forbidden`。                                                                                     |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.rejectJoinResponse"
}-->
```json
{
  "reason": "None | Busy | Forbidden" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "rejectJoinResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
