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
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="aea42-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="aea42-103">Configuring the invitation message</span></span>

<span data-ttu-id="aea42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aea42-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="aea42-105">使用 invitedusermessageinfo 对象允许您配置 [邀请](invitation.md) 邮件。</span><span class="sxs-lookup"><span data-stu-id="aea42-105">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="aea42-106">属性</span><span class="sxs-lookup"><span data-stu-id="aea42-106">Properties</span></span>
| <span data-ttu-id="aea42-107">属性</span><span class="sxs-lookup"><span data-stu-id="aea42-107">Property</span></span>     | <span data-ttu-id="aea42-108">类型</span><span class="sxs-lookup"><span data-stu-id="aea42-108">Type</span></span>   |<span data-ttu-id="aea42-109">说明</span><span class="sxs-lookup"><span data-stu-id="aea42-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aea42-110">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="aea42-110">ccRecipients</span></span>|<span data-ttu-id="aea42-111">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="aea42-111">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="aea42-112">应将邀请邮件发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="aea42-112">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="aea42-113">目前仅支持1个额外的收件人。</span><span class="sxs-lookup"><span data-stu-id="aea42-113">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="aea42-114">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="aea42-114">customizedMessageBody</span></span>|<span data-ttu-id="aea42-115">String</span><span class="sxs-lookup"><span data-stu-id="aea42-115">String</span></span>|<span data-ttu-id="aea42-116">如果不需要默认邮件，则为要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="aea42-116">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="aea42-117">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="aea42-117">messageLanguage</span></span>|<span data-ttu-id="aea42-118">String</span><span class="sxs-lookup"><span data-stu-id="aea42-118">String</span></span>|<span data-ttu-id="aea42-119">要在其中发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="aea42-119">The language you want to send the default message in.</span></span> <span data-ttu-id="aea42-120">如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送邮件。</span><span class="sxs-lookup"><span data-stu-id="aea42-120">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="aea42-121">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="aea42-121">The language format should be in ISO 639.</span></span> <span data-ttu-id="aea42-122">默认值为 en-us。</span><span class="sxs-lookup"><span data-stu-id="aea42-122">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aea42-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aea42-123">JSON representation</span></span>
<span data-ttu-id="aea42-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aea42-124">Here is a JSON representation of the resource</span></span>

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

