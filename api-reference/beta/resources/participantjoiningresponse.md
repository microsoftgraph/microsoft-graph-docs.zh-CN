---
title: participantJoiningResponse 资源类型
description: 包含对参与者加入通知的响应的抽象基类。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bab489be373e03a5b3ded436ebdbfcf910583acc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446635"
---
# <a name="participantjoiningresponse-resource-type"></a>participantJoiningResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含对参与者加入通知的响应的抽象基类。

## <a name="derived-types"></a>派生类型

| 类型                                                   | 说明                                                                                          |
| :----------------------------------------------------- | :--------------------------------------------------------------------                                |
| [acceptJoinResponse](./acceptjoinresponse.md)          | 响应以接受呼叫参与者。                                                           |
| [rejectJoinResponse](./rejectjoinresponse.md)          | 响应以拒绝呼叫参与者。                                                           |
| [inviteNewBotResponse](./invitenewbotresponse.md)      | 响应以传入呼叫通知发送再次发送的参与者加入通知。 |

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

