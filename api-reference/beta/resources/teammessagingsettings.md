---
title: teamMessagingSettings 资源类型
description: 要配置的消息设置和团队中的提及。
ms.openlocfilehash: 51a0fb53079e8fd79f469f022efb2f293e9a6cba
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043536"
---
# <a name="teammessagingsettings-resource-type"></a>teamMessagingSettings 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

要配置的消息设置和[团队](team.md)中的提及。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
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
