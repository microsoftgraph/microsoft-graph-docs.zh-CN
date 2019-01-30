---
title: 配置邀请邮件
description: 使用 invitedUserMessageInfo 对象可以配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643788"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="6f670-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="6f670-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f670-104">使用 invitedUserMessageInfo 对象可以配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="6f670-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="6f670-105">属性</span><span class="sxs-lookup"><span data-stu-id="6f670-105">Properties</span></span>
| <span data-ttu-id="6f670-106">属性</span><span class="sxs-lookup"><span data-stu-id="6f670-106">Property</span></span>     | <span data-ttu-id="6f670-107">类型</span><span class="sxs-lookup"><span data-stu-id="6f670-107">Type</span></span>   |<span data-ttu-id="6f670-108">说明</span><span class="sxs-lookup"><span data-stu-id="6f670-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6f670-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="6f670-109">ccRecipients</span></span>|[<span data-ttu-id="6f670-110">收件人</span><span class="sxs-lookup"><span data-stu-id="6f670-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="6f670-p101">应接收邀请邮件的其他收件人。当前仅支持 1 个其他收件人。</span><span class="sxs-lookup"><span data-stu-id="6f670-p101">Additional recipients the invitation message should be sent to. Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="6f670-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="6f670-113">customizedMessageBody</span></span>|<span data-ttu-id="6f670-114">字符串</span><span class="sxs-lookup"><span data-stu-id="6f670-114">String</span></span>|<span data-ttu-id="6f670-115">在不希望发送默认邮件的情况下，要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="6f670-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="6f670-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="6f670-116">messageLanguage</span></span>|<span data-ttu-id="6f670-117">字符串</span><span class="sxs-lookup"><span data-stu-id="6f670-117">String</span></span>|<span data-ttu-id="6f670-p102">要发送的默认邮件的语言。如果指定了 customizedMessageBody，则忽略此属性，并使用 customizedMessageBody 发送该邮件。语言格式应为 ISO 639 格式。默认为 zh-CN。</span><span class="sxs-lookup"><span data-stu-id="6f670-p102">The language you want to send the default message in. If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody. The language format should be in ISO 639. The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6f670-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6f670-122">JSON representation</span></span>
<span data-ttu-id="6f670-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f670-123">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/invitedusermessageinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
