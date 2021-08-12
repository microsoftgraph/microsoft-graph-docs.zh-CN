---
title: chatInfo 资源类型
description: 有关邮件中Microsoft Teams。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 5ae704998bab3015c265d96c188dbcf8eba4729c4df3a1b8a72f3d5076a7f8b6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180878"
---
# <a name="chatinfo-resource-type"></a>chatInfo 资源类型

命名空间：microsoft.graph

其中包含与会议相关的Microsoft Teams信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| messageId           | String  | 邮件通道中邮件的唯一Microsoft Teams标识符。 |
| replyChainMessageId | String  | 回复邮件的 ID。 |
| threadId            | String  | 主题中主题的唯一Microsoft Teams。 |

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.chatInfo"
}-->
```json
{
  "messageId": "String",
  "replyChainMessageId": "String",
  "threadId": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chatInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

