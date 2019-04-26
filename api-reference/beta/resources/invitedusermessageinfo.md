---
title: 配置邀请邮件
description: 使用 invitedusermessageinfo 对象允许您配置邀请邮件。
localization_priority: Normal
ms.openlocfilehash: fa7ead6938ddfaca78322f56f4638c45d3f2df14
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569968"
---
# <a name="configuring-the-invitation-message"></a><span data-ttu-id="f8e0d-103">配置邀请邮件</span><span class="sxs-lookup"><span data-stu-id="f8e0d-103">Configuring the invitation message</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f8e0d-104">使用 invitedusermessageinfo 对象允许您配置[邀请](invitation.md)邮件。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-104">The invitedUserMessageInfo object allows you to configure the [invitation](invitation.md) message.</span></span>


## <a name="properties"></a><span data-ttu-id="f8e0d-105">属性</span><span class="sxs-lookup"><span data-stu-id="f8e0d-105">Properties</span></span>
| <span data-ttu-id="f8e0d-106">属性</span><span class="sxs-lookup"><span data-stu-id="f8e0d-106">Property</span></span>     | <span data-ttu-id="f8e0d-107">类型</span><span class="sxs-lookup"><span data-stu-id="f8e0d-107">Type</span></span>   |<span data-ttu-id="f8e0d-108">说明</span><span class="sxs-lookup"><span data-stu-id="f8e0d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f8e0d-109">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="f8e0d-109">ccRecipients</span></span>|[<span data-ttu-id="f8e0d-110">收件人</span><span class="sxs-lookup"><span data-stu-id="f8e0d-110">Recipients</span></span>](recipient.md)|<span data-ttu-id="f8e0d-111">应将邀请邮件发送到的其他收件人。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-111">Additional recipients the invitation message should be sent to.</span></span> <span data-ttu-id="f8e0d-112">目前仅支持1个额外的收件人。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-112">Currently only 1 additional recipient is supported.</span></span>|
|<span data-ttu-id="f8e0d-113">customizedMessageBody</span><span class="sxs-lookup"><span data-stu-id="f8e0d-113">customizedMessageBody</span></span>|<span data-ttu-id="f8e0d-114">String</span><span class="sxs-lookup"><span data-stu-id="f8e0d-114">String</span></span>|<span data-ttu-id="f8e0d-115">如果不需要默认邮件, 则为要发送的自定义邮件正文。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-115">Customized message body you want to send if you don't want the default message.</span></span>|
|<span data-ttu-id="f8e0d-116">messageLanguage</span><span class="sxs-lookup"><span data-stu-id="f8e0d-116">messageLanguage</span></span>|<span data-ttu-id="f8e0d-117">String</span><span class="sxs-lookup"><span data-stu-id="f8e0d-117">String</span></span>|<span data-ttu-id="f8e0d-118">要在其中发送默认邮件的语言。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-118">The language you want to send the default message in.</span></span> <span data-ttu-id="f8e0d-119">如果指定了 customizedMessageBody, 则忽略此属性, 并使用 customizedMessageBody 发送邮件。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-119">If the customizedMessageBody is specified, this property is ignored, and the message is sent using the customizedMessageBody.</span></span> <span data-ttu-id="f8e0d-120">语言格式应为 ISO 639。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-120">The language format should be in ISO 639.</span></span> <span data-ttu-id="f8e0d-121">默认值为 en-us。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-121">The default is en-US.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f8e0d-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f8e0d-122">JSON representation</span></span>
<span data-ttu-id="f8e0d-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8e0d-123">Here is a JSON representation of the resource</span></span>

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
