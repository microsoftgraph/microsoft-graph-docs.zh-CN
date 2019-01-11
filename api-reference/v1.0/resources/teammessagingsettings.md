---
title: teamMessagingSettings 资源类型
description: 要配置的消息设置和团队中的提及。
author: nkramer
localization_priority: Normal
ms.openlocfilehash: df80fbb828a400e736b2e8c3b73f949fe6bfd1ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878377"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型



要配置的消息设置和[团队](team.md)中的提及。

## <a name="properties"></a>属性
| 属性     | 类型   |Description|
|:---------------|:--------|:----------|
|allowUserEditMessages|布尔|如果设置为 true，则用户可以编辑他们的邮件。|
|allowUserDeleteMessages|布尔|如果设置为 true，则用户可以删除其邮件。|
|allowOwnerDeleteMessages|布尔|如果设置为 true，则所有者可以删除任何消息。|
|allowTeamMentions|布尔|如果设置为 true，允许提及的 @team。|
|allowChannelMentions|布尔|如果设置为 true，允许提及的 @channel。|

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
<!-- {
  "type": "#page.annotation",
  "description": "team's messagingSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
