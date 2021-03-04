---
title: inviteNewBotResponse 资源类型
description: 包含对请求的响应，请求让参与者加入通知作为传入呼叫通知再次发送到所需位置。
author: yizhenww
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3811c1b5aa6fe21a361cd371ab0b39e6ea00c7b1
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446642"
---
# <a name="invitenewbotresponse-resource-type"></a>inviteNewBotResponse 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含对请求的响应，请求让参与者加入通知作为传入呼叫通知再次发送到所需位置。

## <a name="properties"></a>属性

| 属性         | 类型                            | 说明                                                                                                                                                  |
| :--------------- | :------------------------------ | :----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| inviteUri        | String                          | 接收新传入呼叫通知的 URI。                                                                                                                |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.inviteNewBotResponse"
}-->
```json
{
  "inviteUri": "uri" 
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inviteNewBotResponse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
