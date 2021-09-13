---
title: participantJoiningNotification 资源类型
description: 包含有关加入呼叫的基于策略的参与者的详细信息。
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9e9b0186035e055b06c99fe60a52ca1ff63dc5bc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59036058"
---
# <a name="participantjoiningnotification-resource-type"></a>participantJoiningNotification 资源类型

命名空间：microsoft.graph

包含有关加入呼叫的基于策略的参与者的详细信息。

在基于 [策略](/microsoftteams/teams-recording-policy)的录制方案下，在策略下的参与者加入呼叫之前，会向与具有可用容量来处理新参与者的策略关联的自动程序 `participantJoiningNotification` 发送 。

响应 [负载中的 participantJoiningResponse](participantjoiningResponse.md) 应来自机器人。

## <a name="properties"></a>属性
| 属性       | 类型            | 说明                                                        |
| -------------- | --------------  | -------------------------------------------                        |
| 通话           | [call](call.md) | 包含有关参与者加入事件的详细信息的 call 对象。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.participantJoiningNotification"
}-->
```json
{
  "call": {"@odata.type": "#microsoft.graph.call"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningNotification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
