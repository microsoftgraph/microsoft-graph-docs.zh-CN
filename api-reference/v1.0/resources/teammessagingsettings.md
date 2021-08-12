---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 9818e161e21f78a83023ead66d7b790eadd01bb2737942a383665338d0ec73c4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129958"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型

命名空间：microsoft.graph



设置在团队中配置消息传递和[提及](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowUserEditMessages|Boolean|如果设置为 true，则用户可以编辑其邮件。|
|allowUserDeleteMessages|Boolean|如果设置为 true，用户可以删除其邮件。|
|allowOwnerDeleteMessages|Boolean|如果设置为 true，所有者可以删除任何邮件。|
|allowTeamMentions|Boolean|如果设置为 true，则@team提及。|
|allowChannelMentions|Boolean|如果设置为 true，则@channel提及。|

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

