---
title: 配置邀请邮件
description: 使用 invitedusermessageinfo 对象允许您配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: 458efdade9b5cd7b538ffa3e217ec915dac93ad9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341342"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="9dac3-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="9dac3-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9dac3-104">使用 invitedusermessageinfo 对象允许您配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="9dac3-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="9dac3-105">属性</span><span class="sxs-lookup"><span data-stu-id="9dac3-105">Properties</span></span>
| <span data-ttu-id="9dac3-106">属性</span><span class="sxs-lookup"><span data-stu-id="9dac3-106">Property</span></span>     | <span data-ttu-id="9dac3-107">类型</span><span class="sxs-lookup"><span data-stu-id="9dac3-107">Type</span></span>   |<span data-ttu-id="9dac3-108">说明</span><span class="sxs-lookup"><span data-stu-id="9dac3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dac3-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="9dac3-109">ccRecipients</span></span>|<span data-ttu-id="9dac3-110">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="9dac3-110">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="9dac3-111">应将邀请邮件发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="9dac3-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="9dac3-112">目前仅支持1个额外的收件人。</span><span class="sxs-lookup"><span data-stu-id="9dac3-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="9dac3-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="9dac3-113">customizedMessageBody</span></span>|<span data-ttu-id="9dac3-114">String</span><span class="sxs-lookup"><span data-stu-id="9dac3-114">String</span></span>|<span data-ttu-id="9dac3-115">如果不需要默认邮件, 则为要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="9dac3-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="9dac3-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="9dac3-116">messageLanguage</span></span>|<span data-ttu-id="9dac3-117">String</span><span class="sxs-lookup"><span data-stu-id="9dac3-117">String</span></span>|<span data-ttu-id="9dac3-118">要在其中发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="9dac3-118">The language you want to send the default message in.</span></span> <span data-ttu-id="9dac3-119">如果指定了 customizedMessageBody, 则忽略此属性, 并使用 customizedMessageBody 发送邮件。</span><span class="sxs-lookup"><span data-stu-id="9dac3-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="9dac3-120">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="9dac3-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="9dac3-121">默认值为 en-us。</span><span class="sxs-lookup"><span data-stu-id="9dac3-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dac3-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9dac3-122">JSON representation</span></span>
<span data-ttu-id="9dac3-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dac3-123">Here is a JSON representation of the resource</span></span>

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
