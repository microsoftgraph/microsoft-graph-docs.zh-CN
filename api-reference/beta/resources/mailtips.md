---
title: 邮件提示资源类型
description: '有关收件人的信息性消息, 在用户撰写邮件时向其显示。 例如, 外出邮件 '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 11e64c09a90d130b7656d4e87770e6df3fb67408
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562609"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="158ef-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="158ef-104">mailTips resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="158ef-105">有关收件人的信息性消息, 在用户撰写邮件时向其显示。</span><span class="sxs-lookup"><span data-stu-id="158ef-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="158ef-106">例如, 外出邮件作为邮件收件人的自动答复。</span><span class="sxs-lookup"><span data-stu-id="158ef-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="158ef-107">属性</span><span class="sxs-lookup"><span data-stu-id="158ef-107">Properties</span></span>
| <span data-ttu-id="158ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="158ef-108">Property</span></span>     | <span data-ttu-id="158ef-109">类型</span><span class="sxs-lookup"><span data-stu-id="158ef-109">Type</span></span>   |<span data-ttu-id="158ef-110">说明</span><span class="sxs-lookup"><span data-stu-id="158ef-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="158ef-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="158ef-111">automaticReplies</span></span> | [<span data-ttu-id="158ef-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="158ef-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="158ef-113">"自动答复" 的邮件提示 (如果收件人已设置)。</span><span class="sxs-lookup"><span data-stu-id="158ef-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="158ef-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="158ef-114">customMailTip</span></span> | <span data-ttu-id="158ef-115">String</span><span class="sxs-lookup"><span data-stu-id="158ef-115">String</span></span> | <span data-ttu-id="158ef-116">可在收件人邮箱上设置的自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="158ef-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="158ef-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="158ef-117">deliveryRestricted</span></span>| <span data-ttu-id="158ef-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="158ef-118">Boolean</span></span> | <span data-ttu-id="158ef-119">收件人邮箱是否受到限制, 例如, 仅接受来自预定义的发件人列表的邮件、拒绝来自预定义的发件人列表的邮件, 还是仅接受来自已验证的发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="158ef-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="158ef-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="158ef-120">emailAddress</span></span> | [<span data-ttu-id="158ef-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="158ef-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="158ef-122">要获取其邮件提示的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="158ef-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="158ef-123">error</span><span class="sxs-lookup"><span data-stu-id="158ef-123">error</span></span> | [<span data-ttu-id="158ef-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="158ef-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="158ef-125">[getMailTips](../api/user-getmailtips.md)操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="158ef-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="158ef-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="158ef-126">externalMemberCount</span></span> | <span data-ttu-id="158ef-127">Int32</span><span class="sxs-lookup"><span data-stu-id="158ef-127">Int32</span></span> | <span data-ttu-id="158ef-128">如果收件人是通讯组列表, 则为外部成员的数量。</span><span class="sxs-lookup"><span data-stu-id="158ef-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="158ef-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="158ef-129">isModerated</span></span> |<span data-ttu-id="158ef-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="158ef-130">Boolean</span></span>  | <span data-ttu-id="158ef-131">向收件人发送邮件是否需要审批。</span><span class="sxs-lookup"><span data-stu-id="158ef-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="158ef-132">例如, 如果收件人是一个大型通讯组列表, 并且已将仲裁人设置为审批发送到该通讯组列表的邮件, 或者向收件人发送邮件时需要对收件人的经理进行审批。</span><span class="sxs-lookup"><span data-stu-id="158ef-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="158ef-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="158ef-133">mailboxFull</span></span> | <span data-ttu-id="158ef-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="158ef-134">Boolean</span></span> | <span data-ttu-id="158ef-135">收件人的邮箱完整状态。</span><span class="sxs-lookup"><span data-stu-id="158ef-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="158ef-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="158ef-136">maxMessageSize</span></span> | <span data-ttu-id="158ef-137">Int32</span><span class="sxs-lookup"><span data-stu-id="158ef-137">Int32</span></span> | <span data-ttu-id="158ef-138">已为收件人的组织或邮箱配置的最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="158ef-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="158ef-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="158ef-139">recipientScope</span></span> | <span data-ttu-id="158ef-140">String</span><span class="sxs-lookup"><span data-stu-id="158ef-140">String</span></span> | <span data-ttu-id="158ef-141">收件人的范围。</span><span class="sxs-lookup"><span data-stu-id="158ef-141">The scope of the recipient.</span></span> <span data-ttu-id="158ef-142">可取值为：`none`、`internal`、`external`、`externalPartner` 或 `externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="158ef-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="158ef-143">例如, 管理员可以将其他组织设置为其 "合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="158ef-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="158ef-144">如果管理员希望某些范围能够访问某些邮件提示, 则该范围很有用。</span><span class="sxs-lookup"><span data-stu-id="158ef-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="158ef-145">对于发件人来说, 通知他们其邮件可能会离开组织, 从而帮助他们做出正确的措辞、语气和内容决策。</span><span class="sxs-lookup"><span data-stu-id="158ef-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="158ef-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="158ef-146">recipientSuggestions</span></span> | <span data-ttu-id="158ef-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="158ef-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="158ef-148">根据以前的上下文显示在同一邮件中建议的收件人。</span><span class="sxs-lookup"><span data-stu-id="158ef-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="158ef-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="158ef-149">totalMemberCount</span></span> | <span data-ttu-id="158ef-150">Int32</span><span class="sxs-lookup"><span data-stu-id="158ef-150">Int32</span></span> | <span data-ttu-id="158ef-151">如果收件人是通讯组列表, 则为成员数量。</span><span class="sxs-lookup"><span data-stu-id="158ef-151">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="158ef-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="158ef-152">JSON representation</span></span>

<span data-ttu-id="158ef-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="158ef-153">Here is a JSON representation of the resource.</span></span>

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
