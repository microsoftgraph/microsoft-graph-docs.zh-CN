---
title: tokenMeetingInfo 资源类型
description: TokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e34a10b9cd0fb09ff29c2d3373ad51a92109dcea
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40865757"
---
# <a name="tokenmeetinginfo-resource-type"></a>tokenMeetingInfo 资源类型

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
