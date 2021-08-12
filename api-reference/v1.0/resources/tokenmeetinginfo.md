---
title: tokenMeetingInfo 资源类型
description: tokenMeetingInfo 类型。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 269cd5589539cb63b20d61e5103a273a083882a4ffa89446e1c6629444d1b9c5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159860"
---
# <a name="tokenmeetinginfo-resource-type"></a>tokenMeetingInfo 资源类型

命名空间：microsoft.graph

这是允许你加入现有会议令牌信息。 这是作为传入呼叫通知的一部分获取的。 

如果呼叫断开，此信息可以帮助您重新加入该呼叫。

## <a name="properties"></a>属性

| 属性                     | 类型    | 说明                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| 令牌                        | String  | 用于加入调用的令牌。                                                 |

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

