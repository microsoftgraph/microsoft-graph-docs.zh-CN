---
title: inviteNewBotResponse 资源类型
description: 包含对请求的响应，请求让参与者加入通知作为传入呼叫通知再次发送到所需位置。
author: yizhenww
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: cca303fff854fddff56f6bc8ffd30160f390401c
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084403"
---
# <a name="invitenewbotresponse-resource-type"></a>inviteNewBotResponse 资源类型

命名空间：microsoft.graph

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
