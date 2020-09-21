---
title: 配置邀请邮件
description: 使用 invitedusermessageinfo 对象允许您配置邀请邮件。
localization_priority: Normal
author: elisolMS
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c4946f405bf23bf9779d05a470c90fd6936b900
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47967497"
---
# <a name="configuring-the-invitation-message"></a>配置邀请邮件

命名空间：microsoft.graph

使用 invitedusermessageinfo 对象允许您配置 [邀请](invitation.md) 邮件。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ccRecipients|[Recipient](recipient.md) collection|应将邀请邮件发送到的其他收件人。 目前仅支持1个额外的收件人。|
|customizedMessageBody|String|如果不需要默认邮件，则为要发送的自定义邮件正文。|
|messageLanguage|String|要在其中发送默认邮件的语言。 如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送邮件。 语言格式应为 ISO 639。 默认值为 en-us。|

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
<!-- {
  "type": "#page.annotation",
  "description": "invitedUserMessageInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

