---
title: 配置邀请邮件
description: invitedUserMessageInfo 对象允许您配置邀请消息。
ms.localizationpriority: medium
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 473e043da7669cc07e79fdf3a06edb0d36f657ba
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084417"
---
# <a name="configuring-the-invitation-message"></a>配置邀请邮件

命名空间：microsoft.graph

invitedUserMessageInfo 对象允许您配置 [邀请](invitation.md) 消息。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ccRecipients|[Recipient](recipient.md) collection|邀请邮件应发送到的其他收件人。 目前仅支持另外 1 个收件人。|
|customizedMessageBody|String|如果不希望使用默认邮件，则发送的自定义邮件正文。|
|messageLanguage|String|要发送默认邮件的语言。 如果指定了 customizedMessageBody，则忽略此属性，并且使用 customizedMessageBody 发送消息。 语言格式应为 ISO 639。 默认值为 en-US。|

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

