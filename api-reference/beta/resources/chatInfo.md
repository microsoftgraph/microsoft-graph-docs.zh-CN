---
title: chatInfo 资源类型
description: 包含与 Microsoft 团队会议相关的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8602301af0de458f07ab5a9c0af00ec8578c3a61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507731"
---
# <a name="chatinfo-resource-type"></a>chatInfo 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

包含与 Microsoft 团队会议相关的信息。

## <a name="properties"></a>属性

| 属性            | 类型    | 说明|
|:--------------------|:--------|:-----------|
| messageId           | String  | Microsoft 团队频道中的邮件的唯一标识符。 |
| replyChainMessageId | String  | 答复邮件的 ID。 |
| threadId            | String  | Microsoft 团队中的线程的唯一标识符。 |

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
