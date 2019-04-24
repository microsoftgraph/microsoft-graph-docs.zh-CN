---
title: 配置邀请邮件
description: 使用 invitedusermessageinfo 对象允许您配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: 06be157e61fd6d466cc2b18546bb29762d0133a8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585116"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="ac445-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="ac445-103">Configuring the invitation message</span></span>

<span data-ttu-id="ac445-104">使用 invitedusermessageinfo 对象允许您配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="ac445-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="ac445-105">属性</span><span class="sxs-lookup"><span data-stu-id="ac445-105">Properties</span></span>
| <span data-ttu-id="ac445-106">属性</span><span class="sxs-lookup"><span data-stu-id="ac445-106">Property</span></span>     | <span data-ttu-id="ac445-107">类型</span><span class="sxs-lookup"><span data-stu-id="ac445-107">Type</span></span>   |<span data-ttu-id="ac445-108">说明</span><span class="sxs-lookup"><span data-stu-id="ac445-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac445-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="ac445-109">ccRecipients</span></span>|<span data-ttu-id="ac445-110">[Recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="ac445-110">[Recipient](recipient.md) collection</span></span>|<span data-ttu-id="ac445-111">应将邀请邮件发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="ac445-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="ac445-112">目前仅支持1个额外的收件人。</span><span class="sxs-lookup"><span data-stu-id="ac445-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="ac445-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="ac445-113">customizedMessageBody</span></span>|<span data-ttu-id="ac445-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ac445-114">String</span></span>|<span data-ttu-id="ac445-115">如果不需要默认邮件, 则为要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="ac445-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="ac445-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="ac445-116">messageLanguage</span></span>|<span data-ttu-id="ac445-117">字符串</span><span class="sxs-lookup"><span data-stu-id="ac445-117">String</span></span>|<span data-ttu-id="ac445-118">要在其中发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="ac445-118">The language you want to send the default message in.</span></span> <span data-ttu-id="ac445-119">如果指定了 customizedMessageBody, 则忽略此属性, 并使用 customizedMessageBody 发送邮件。</span><span class="sxs-lookup"><span data-stu-id="ac445-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="ac445-120">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="ac445-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="ac445-121">默认值为 en-us。</span><span class="sxs-lookup"><span data-stu-id="ac445-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ac445-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ac445-122">JSON representation</span></span>
<span data-ttu-id="ac445-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ac445-123">Here is a JSON representation of the resource</span></span>

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
