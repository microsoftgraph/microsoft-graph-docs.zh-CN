---
title: rejectJoinResponse 资源类型
description: 包含拒绝尝试加入会议的参与者的响应。
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: f16c061d6652f68ca27744d32e1203ef46c1d1fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044242"
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
