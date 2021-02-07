---
title: 配置邀请邮件
description: invitedUserMessageInfo 对象允许你配置邀请邮件。
localization_priority: Normal
author: elisolMS
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: d44542b26fd1c1ffb7b70dcfc019ada6f0cc02f5
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129721"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="a1a92-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="a1a92-103">Configuring the invitation message</span></span>

<span data-ttu-id="a1a92-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1a92-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1a92-105">invitedUserMessageInfo 对象允许你配置 [邀请](invitation.md) 邮件。</span><span class="sxs-lookup"><span data-stu-id="a1a92-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="a1a92-106">属性</span><span class="sxs-lookup"><span data-stu-id="a1a92-106">Properties</span></span>
| <span data-ttu-id="a1a92-107">属性</span><span class="sxs-lookup"><span data-stu-id="a1a92-107">Property</span></span>     | <span data-ttu-id="a1a92-108">类型</span><span class="sxs-lookup"><span data-stu-id="a1a92-108">Type</span></span>   |<span data-ttu-id="a1a92-109">说明</span><span class="sxs-lookup"><span data-stu-id="a1a92-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1a92-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="a1a92-110">ccRecipients</span></span>|<span data-ttu-id="a1a92-111">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="a1a92-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="a1a92-112">邀请邮件应发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="a1a92-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="a1a92-113">当前仅支持另外 1 个收件人。</span><span class="sxs-lookup"><span data-stu-id="a1a92-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="a1a92-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="a1a92-114">customizedMessageBody</span></span>|<span data-ttu-id="a1a92-115">String</span><span class="sxs-lookup"><span data-stu-id="a1a92-115">String</span></span>|<span data-ttu-id="a1a92-116">不需要默认邮件时要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="a1a92-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="a1a92-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="a1a92-117">messageLanguage</span></span>|<span data-ttu-id="a1a92-118">String</span><span class="sxs-lookup"><span data-stu-id="a1a92-118">String</span></span>|<span data-ttu-id="a1a92-119">要发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="a1a92-119">The language you want to send the default message in.</span></span> <span data-ttu-id="a1a92-120">如果指定了 customizedMessageBody，则忽略此属性，并且使用 customizedMessageBody 发送邮件。</span><span class="sxs-lookup"><span data-stu-id="a1a92-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="a1a92-121">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="a1a92-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="a1a92-122">默认值为 en-US。</span><span class="sxs-lookup"><span data-stu-id="a1a92-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a1a92-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a1a92-123">JSON representation</span></span>
<span data-ttu-id="a1a92-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1a92-124">Here is a JSON representation of the resource</span></span>

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

