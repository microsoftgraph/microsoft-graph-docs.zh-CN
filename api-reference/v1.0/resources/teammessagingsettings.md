---
title: teamMessagingSettings 资源类型
description: 用于配置团队中的消息传递和提及的设置。
author: nkramer
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 08af21e988862a4d6b459953e6d1a1fd5554da36
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59049485"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型

命名空间：microsoft.graph



设置在团队中配置消息传递和[提及](team.md)。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|allowUserEditMessages|布尔值|如果设置为 true，则用户可以编辑其邮件。|
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

