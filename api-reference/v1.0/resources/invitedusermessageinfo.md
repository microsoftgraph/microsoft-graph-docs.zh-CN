---
title: 配置邀请邮件
description: invitedUserMessageInfo 对象允许您配置邀请消息。
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 5b20eb15cfc8eb2ae248d87e5ae61ffa0d5ea08d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941377"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="ae757-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="ae757-103">Configuring the invitation message</span></span>

<span data-ttu-id="ae757-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ae757-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ae757-105">invitedUserMessageInfo 对象允许您配置 [邀请](invitation.md) 消息。</span><span class="sxs-lookup"><span data-stu-id="ae757-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="ae757-106">属性</span><span class="sxs-lookup"><span data-stu-id="ae757-106">Properties</span></span>
| <span data-ttu-id="ae757-107">属性</span><span class="sxs-lookup"><span data-stu-id="ae757-107">Property</span></span>     | <span data-ttu-id="ae757-108">类型</span><span class="sxs-lookup"><span data-stu-id="ae757-108">Type</span></span>   |<span data-ttu-id="ae757-109">说明</span><span class="sxs-lookup"><span data-stu-id="ae757-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae757-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="ae757-110">ccRecipients</span></span>|<span data-ttu-id="ae757-111">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ae757-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="ae757-112">邀请邮件应发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="ae757-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="ae757-113">目前仅支持另外 1 个收件人。</span><span class="sxs-lookup"><span data-stu-id="ae757-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="ae757-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="ae757-114">customizedMessageBody</span></span>|<span data-ttu-id="ae757-115">String</span><span class="sxs-lookup"><span data-stu-id="ae757-115">String</span></span>|<span data-ttu-id="ae757-116">如果不希望使用默认邮件，则发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="ae757-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="ae757-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="ae757-117">messageLanguage</span></span>|<span data-ttu-id="ae757-118">String</span><span class="sxs-lookup"><span data-stu-id="ae757-118">String</span></span>|<span data-ttu-id="ae757-119">要发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="ae757-119">The language you want to send the default message in.</span></span> <span data-ttu-id="ae757-120">如果指定了 customizedMessageBody，则忽略此属性，并且使用 customizedMessageBody 发送消息。</span><span class="sxs-lookup"><span data-stu-id="ae757-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="ae757-121">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="ae757-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="ae757-122">默认值为 en-US。</span><span class="sxs-lookup"><span data-stu-id="ae757-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae757-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ae757-123">JSON representation</span></span>
<span data-ttu-id="ae757-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ae757-124">Here is a JSON representation of the resource</span></span>

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

