---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 27ef5062e84f20dc1dbf6be11020f421871fbc09
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033836"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型



用于配置[团队](team.md)中的消息传递和提及的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|如果设置为 true, 则用户可以编辑其邮件。|
|allowUserDeleteMessages|Boolean|如果设置为 true, 则用户可以删除其邮件。|
|allowOwnerDeleteMessages|Boolean|如果设置为 true, 则所有者可以删除任何邮件。|
|allowTeamMentions|Boolean|如果设置为 true, 则允许 @team 提及。|
|allowChannelMentions|Boolean|如果设置为 true, 则允许 @channel 提及。|

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
