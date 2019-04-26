---
title: tokenMeetingInfo 资源类型
description: tokenMeetingInfo 类型。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 38a5aae17cf4364a1cfd58680c2e7b9437cf0e40
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345498"
---
# <a name="tokenmeetinginfo-resource-type"></a>tokenMeetingInfo 资源类型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

tokenMeetingInfo 类型。

## <a name="properties"></a>属性

| 属性                     | 类型    | 说明                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| allowConversationWithoutHost | Boolean | 指示会话离开的主机后是否可以继续会话。 |
| token                        | String  | 要加入/激活会议的令牌。                                        |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a>示例

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
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
