---
title: 配置邀请邮件
description: 使用 invitedUserMessageInfo 对象可以配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507780"
---
# <a name="configuring-the-invitation-message"></a>配置邀请邮件

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ccRecipients|[收件人](recipient.md)|应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。|
|customizedMessageBody|String|在不希望发送默认邮件的情况下，要发送的自定义邮件正文。|
|messageLanguage|字符串|要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。

<!-- {"blockType": "resource", "@odata.type": "microsoft.graph.invitedUserMessageInfo"} -->
```json
{
  "ccRecipients": [ {"@odata.type": "microsoft.graph.recipient"} ],
  "customizedMessageBody": "string",
  "messageLanguage": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
