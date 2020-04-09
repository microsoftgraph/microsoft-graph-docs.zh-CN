---
title: 配置邀请邮件
description: 使用 invitedusermessageinfo 对象允许您配置邀请邮件。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: elisolMS
ms.openlocfilehash: 7b2d4e25dc85f1140ecba9ab9d0365cc4e842be6
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200087"
---
# <a name="configuring-the-invitation-message"></a>配置邀请邮件

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用 invitedusermessageinfo 对象允许您配置[邀请](invitation.md)邮件。


## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|ccRecipients|[recipient](recipient.md) collection|应将邀请邮件发送到的其他收件人。 目前仅支持1个额外的收件人。|
|customizedMessageBody|字符串|如果不需要默认邮件，则为要发送的自定义邮件正文。|
|messageLanguage|字符串|要在其中发送默认邮件的语言。 如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送邮件。 语言格式应为 ISO 639。 默认值为 en-us。|

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
  "suppressions": []
}
-->
