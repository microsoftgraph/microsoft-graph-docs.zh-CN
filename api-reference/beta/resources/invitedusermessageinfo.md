---
title: 配置邀请邮件
description: 使用 invitedUserMessageInfo 对象可以配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: f8a6dd118f1774320e3fe8327d284dac1141fc55
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874121"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="bb8f0-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="bb8f0-103">Configuring the invitation message</span></span>

> <span data-ttu-id="bb8f0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb8f0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bb8f0-106">使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-106">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="bb8f0-107">属性</span><span class="sxs-lookup"><span data-stu-id="bb8f0-107">Properties</span></span>
| <span data-ttu-id="bb8f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb8f0-108">Property</span></span>     | <span data-ttu-id="bb8f0-109">类型</span><span class="sxs-lookup"><span data-stu-id="bb8f0-109">Type</span></span>   |<span data-ttu-id="bb8f0-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb8f0-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb8f0-111">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="bb8f0-111">ccRecipients</span></span>|[<span data-ttu-id="bb8f0-112">收件人</span><span class="sxs-lookup"><span data-stu-id="bb8f0-112">Recipients</span></span>](recipient.md)|<span data-ttu-id="bb8f0-p102">应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-p102">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="bb8f0-115">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="bb8f0-115">customizedMessageBody</span></span>|<span data-ttu-id="bb8f0-116">字符串</span><span class="sxs-lookup"><span data-stu-id="bb8f0-116">String</span></span>|<span data-ttu-id="bb8f0-117">在不希望发送默认邮件的情况下，要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-117">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="bb8f0-118">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="bb8f0-118">messageLanguage</span></span>|<span data-ttu-id="bb8f0-119">字符串</span><span class="sxs-lookup"><span data-stu-id="bb8f0-119">String</span></span>|<span data-ttu-id="bb8f0-p103">要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-p103">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bb8f0-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb8f0-124">JSON representation</span></span>
<span data-ttu-id="bb8f0-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb8f0-125">Here is a JSON representation of the resource</span></span>

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
