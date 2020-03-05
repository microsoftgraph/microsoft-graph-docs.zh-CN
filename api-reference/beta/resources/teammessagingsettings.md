---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 213a8d388b80a4b35d26afc0071445a8ac6095b9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519930"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型

命名空间： microsoft. graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用于配置[团队](team.md)中的消息传递和提及的设置。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowUserEditMessages|布尔|如果设置为 true，则用户可以编辑其邮件。|
|allowUserDeleteMessages|布尔|如果设置为 true，则用户可以删除其邮件。|
|allowOwnerDeleteMessages|布尔|如果设置为 true，则所有者可以删除任何邮件。|
|allowTeamMentions|布尔|如果设置为 true，则允许 @team 提及。|
|allowChannelMentions|布尔|如果设置为 true，则允许 @channel 提及。|

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
