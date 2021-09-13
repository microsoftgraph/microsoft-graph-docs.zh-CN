---
title: chatInfo 资源类型
description: 有关邮件中Microsoft Teams。
author: ananmishr
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bc548c9f107232368b43aaeb154db2cf5e2cc517
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59109428"
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

