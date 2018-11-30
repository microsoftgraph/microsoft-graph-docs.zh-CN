---
title: 配置邀请邮件
description: 使用 invitedUserMessageInfo 对象可以配置邀请邮件。
ms.openlocfilehash: c8258d2b90d1aa5f5081b271ccc70fcb7408b132
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010834"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="06438-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="06438-103">Configuring the invitation message</span></span>

<span data-ttu-id="06438-104">使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="06438-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="06438-105">属性</span><span class="sxs-lookup"><span data-stu-id="06438-105">Properties</span></span>
| <span data-ttu-id="06438-106">属性</span><span class="sxs-lookup"><span data-stu-id="06438-106">Property</span></span>     | <span data-ttu-id="06438-107">类型</span><span class="sxs-lookup"><span data-stu-id="06438-107">Type</span></span>   |<span data-ttu-id="06438-108">说明</span><span class="sxs-lookup"><span data-stu-id="06438-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06438-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="06438-109">ccRecipients</span></span>|<span data-ttu-id="06438-110">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="06438-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="06438-p101">应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。</span><span class="sxs-lookup"><span data-stu-id="06438-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="06438-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="06438-113">customizedMessageBody</span></span>|<span data-ttu-id="06438-114">字符串</span><span class="sxs-lookup"><span data-stu-id="06438-114">String</span></span>|<span data-ttu-id="06438-115">在不希望发送默认邮件的情况下，要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="06438-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="06438-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="06438-116">messageLanguage</span></span>|<span data-ttu-id="06438-117">字符串</span><span class="sxs-lookup"><span data-stu-id="06438-117">String</span></span>|<span data-ttu-id="06438-p102">要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。</span><span class="sxs-lookup"><span data-stu-id="06438-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="06438-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06438-122">JSON representation</span></span>
<span data-ttu-id="06438-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06438-123">Here is a JSON representation of the resource</span></span>

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
