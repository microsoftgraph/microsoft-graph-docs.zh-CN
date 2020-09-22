---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 352fc5bc8a8794a455a84d729bb3b2cea6ad34f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48046627"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于配置 [团队](team.md)中的消息传递和提及的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|如果设置为 true，则用户可以编辑其邮件。|
|allowUserDeleteMessages|Boolean|如果设置为 true，则用户可以删除其邮件。|
|allowOwnerDeleteMessages|Boolean|如果设置为 true，则所有者可以删除任何邮件。|
|allowTeamMentions|Boolean|如果设置为 true，则允许 @team 提及。|
|allowChannelMentions|Boolean|如果设置为 true，则允许 @channel 提及。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.teamMessagingSettings"
}-->

```json
{
  "allowUserEditMessages": true,
  "allowUserDeleteMessages": true,
  "allowOwnerDeleteMessages": true,
  "allowTeamMentions": true,
  "allowChannelMentions": true    
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


