---
title: participantJoiningResponse 资源类型
description: 包含对参与者加入通知的响应的抽象基类。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ed48569a942a8b70fdf8fbbeeadb2921623f1a77db55acb948fb61d7dd778ec3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54141397"
---
# <a name="participantjoiningresponse-resource-type"></a>participantJoiningResponse 资源类型

命名空间：microsoft.graph

包含对参与者加入通知的响应的抽象基类。

## <a name="derived-types"></a>派生类型

| 类型                                                   | 说明                                                                                          |
| :----------------------------------------------------- | :--------------------------------------------------------------------                                |
| [acceptJoinResponse](./acceptjoinresponse.md)          | 接受呼叫参与者的响应。                                                           |
| [rejectJoinResponse](./rejectjoinresponse.md)          | 对拒绝呼叫参与者的响应。                                                           |
| [inviteNewBotResponse](./invitenewbotresponse.md)      | 对请求参与者加入通知的响应作为传入呼叫通知再次发送。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "abstract": true,
  "@odata.type": "microsoft.graph.participantJoiningResponse"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantJoiningResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
