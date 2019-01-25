---
title: 邮件提示资源类型
description: '有关提示性消息收件人，它们撰写邮件时向用户显示。 例如，-外出消息 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508410"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="1e3e0-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="1e3e0-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e3e0-105">有关提示性消息收件人，它们撰写邮件时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="1e3e0-106">例如，作为自动回复邮件收件人-外出邮件。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="1e3e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e3e0-107">Properties</span></span>
| <span data-ttu-id="1e3e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e3e0-108">Property</span></span>     | <span data-ttu-id="1e3e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="1e3e0-109">Type</span></span>   |<span data-ttu-id="1e3e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e3e0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1e3e0-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="1e3e0-111">automaticReplies</span></span> | [<span data-ttu-id="1e3e0-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="1e3e0-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="1e3e0-113">如果已被收件人设置，邮件自动回复的提示。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="1e3e0-114">CustomMailTip</span><span class="sxs-lookup"><span data-stu-id="1e3e0-114">customMailTip</span></span> | <span data-ttu-id="1e3e0-115">String</span><span class="sxs-lookup"><span data-stu-id="1e3e0-115">String</span></span> | <span data-ttu-id="1e3e0-116">可在收件人的邮箱中设置自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="1e3e0-117">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="1e3e0-117">deliveryRestricted</span></span>| <span data-ttu-id="1e3e0-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e3e0-118">Boolean</span></span> | <span data-ttu-id="1e3e0-119">收件人的邮箱是否受限制，例如，接受从预定义列表的发件人的邮件拒绝来自发件人的预定义列表的邮件，或接受来自仅经过身份验证发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="1e3e0-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1e3e0-120">emailAddress</span></span> | [<span data-ttu-id="1e3e0-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="1e3e0-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="1e3e0-122">若要获取的邮件提示收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="1e3e0-123">error</span><span class="sxs-lookup"><span data-stu-id="1e3e0-123">error</span></span> | [<span data-ttu-id="1e3e0-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="1e3e0-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="1e3e0-125">在[getMailTips](../api/user-getmailtips.md)操作过程中出现错误。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="1e3e0-126">ExternalMemberCount</span><span class="sxs-lookup"><span data-stu-id="1e3e0-126">externalMemberCount</span></span> | <span data-ttu-id="1e3e0-127">Int32</span><span class="sxs-lookup"><span data-stu-id="1e3e0-127">Int32</span></span> | <span data-ttu-id="1e3e0-128">如果收件人是通讯组列表的外部成员的数目。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="1e3e0-129">IsModerated</span><span class="sxs-lookup"><span data-stu-id="1e3e0-129">isModerated</span></span> |<span data-ttu-id="1e3e0-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e3e0-130">Boolean</span></span>  | <span data-ttu-id="1e3e0-131">是否向收件人发送邮件需要审批。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="1e3e0-132">例如，如果收件人是大型通讯组列表和审阅者已设置最多批准邮件发送到该通讯组列表，或如果发送给邮件收件人需要审批的收件人的经理。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="1e3e0-133">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="1e3e0-133">mailboxFull</span></span> | <span data-ttu-id="1e3e0-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e3e0-134">Boolean</span></span> | <span data-ttu-id="1e3e0-135">收件人邮箱完全状态。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="1e3e0-136">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="1e3e0-136">maxMessageSize</span></span> | <span data-ttu-id="1e3e0-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1e3e0-137">Int32</span></span> | <span data-ttu-id="1e3e0-138">收件人的组织或邮箱已配置最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="1e3e0-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="1e3e0-139">recipientScope</span></span> | <span data-ttu-id="1e3e0-140">String</span><span class="sxs-lookup"><span data-stu-id="1e3e0-140">String</span></span> | <span data-ttu-id="1e3e0-141">收件人范围。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-141">The scope of the recipient.</span></span> <span data-ttu-id="1e3e0-142">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="1e3e0-143">例如，管理员可以设置其他组织为其"合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="1e3e0-144">如果管理员希望某些邮件提示可对特定范围有用范围。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="1e3e0-145">也很有用，告知人的邮件可能离开组织，以帮助其选择正确决定哪些措词、 语气和内容的发件人。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="1e3e0-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="1e3e0-146">recipientSuggestions</span></span> | <span data-ttu-id="1e3e0-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="1e3e0-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="1e3e0-148">收件人建议基于以前上下文它们出现在相同的邮件。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="1e3e0-149">TotalMemberCount</span><span class="sxs-lookup"><span data-stu-id="1e3e0-149">totalMemberCount</span></span> | <span data-ttu-id="1e3e0-150">Int32</span><span class="sxs-lookup"><span data-stu-id="1e3e0-150">Int32</span></span> | <span data-ttu-id="1e3e0-151">如果收件人是通讯组列表成员的数目。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1e3e0-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e3e0-152">JSON representation</span></span>

<span data-ttu-id="1e3e0-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e3e0-153">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "automaticReplies",
    "customMailTip",
    "deliveryRestricted",
    "emailAddress",
    "error",
    "externalMemberCount",
    "isModerated",
    "mailboxFull",
    "maxMessageSize",
    "recipientScope",
    "recipientSuggestions",
    "totalMemberCount"
  ],
  "@odata.type": "microsoft.graph.mailTips"
}-->

```json
{
  "automaticReplies": {"@odata.type": "microsoft.graph.automaticRepliesMailTips"},
  "customMailTip": "string",
  "deliveryRestricted": "boolean",
  "emailAddress": {"@odata.type": "microsoft.graph.emailAddress"},
  "error": {"@odata.type": "microsoft.graph.mailTipsError"},
  "externalMemberCount": 1024,
  "isModerated": "boolean",
  "mailboxFull": "boolean",
  "maxMessageSize": 1024,
  "recipientScope": "string",
  "recipientSuggestions": [{"@odata.type": "microsoft.graph.recipient"}],
  "totalMemberCount": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mailtips.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
