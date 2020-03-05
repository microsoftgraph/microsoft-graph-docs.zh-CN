---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 742961893d4180da861965d818b5c0a997f0f50c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519664"
---
# <a name="tokenmeetinginfo-resource-type"></a>tokenMeetingInfo 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

这是允许你加入现有会议的令牌信息。 这是作为传入呼叫通知的一部分获取的。 

在断开呼叫的情况下，此信息可以帮助您重新加入该呼叫。

## <a name="properties"></a>属性

| 属性                     | 类型    | 说明                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| 令牌                        | String  | 用于加入呼叫的令牌。                                                 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
    "token": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
