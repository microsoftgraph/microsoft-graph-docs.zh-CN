---
title: 邮件提示资源类型
description: '有关提示性消息收件人，它们撰写邮件时向用户显示。 例如，-外出消息 '
localization_priority: Normal
ms.openlocfilehash: 0506d10ad4b1c5eb473b04a30eb8d48334685574
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891691"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="6d5b1-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="6d5b1-104">mailTips resource type</span></span>

<span data-ttu-id="6d5b1-105">有关提示性消息收件人，它们撰写邮件时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-105">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="6d5b1-106">例如，作为自动回复邮件收件人-外出邮件。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-106">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="6d5b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="6d5b1-107">Properties</span></span>
| <span data-ttu-id="6d5b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="6d5b1-108">Property</span></span>     | <span data-ttu-id="6d5b1-109">类型</span><span class="sxs-lookup"><span data-stu-id="6d5b1-109">Type</span></span>   |<span data-ttu-id="6d5b1-110">Description</span><span class="sxs-lookup"><span data-stu-id="6d5b1-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6d5b1-111">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="6d5b1-111">automaticReplies</span></span> | [<span data-ttu-id="6d5b1-112">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="6d5b1-112">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="6d5b1-113">如果已被收件人设置，邮件自动回复的提示。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-113">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="6d5b1-114">customMailTip</span><span class="sxs-lookup"><span data-stu-id="6d5b1-114">customMailTip</span></span> | <span data-ttu-id="6d5b1-115">字符串</span><span class="sxs-lookup"><span data-stu-id="6d5b1-115">String</span></span> | <span data-ttu-id="6d5b1-116">可在收件人的邮箱中设置自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-116">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="6d5b1-117">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="6d5b1-117">deliveryRestricted</span></span>| <span data-ttu-id="6d5b1-118">布尔</span><span class="sxs-lookup"><span data-stu-id="6d5b1-118">Boolean</span></span> | <span data-ttu-id="6d5b1-119">收件人的邮箱是否受限制，例如，接受从预定义列表的发件人的邮件拒绝来自发件人的预定义列表的邮件，或接受来自仅经过身份验证发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-119">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="6d5b1-120">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6d5b1-120">emailAddress</span></span> | [<span data-ttu-id="6d5b1-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="6d5b1-121">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="6d5b1-122">若要获取的邮件提示收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-122">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="6d5b1-123">error</span><span class="sxs-lookup"><span data-stu-id="6d5b1-123">error</span></span> | [<span data-ttu-id="6d5b1-124">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="6d5b1-124">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="6d5b1-125">在[getMailTips](../api/user-getmailtips.md)操作过程中出现错误。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-125">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="6d5b1-126">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="6d5b1-126">externalMemberCount</span></span> | <span data-ttu-id="6d5b1-127">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b1-127">Int32</span></span> | <span data-ttu-id="6d5b1-128">如果收件人是通讯组列表的外部成员的数目。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-128">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="6d5b1-129">isModerated</span><span class="sxs-lookup"><span data-stu-id="6d5b1-129">isModerated</span></span> |<span data-ttu-id="6d5b1-130">布尔</span><span class="sxs-lookup"><span data-stu-id="6d5b1-130">Boolean</span></span>  | <span data-ttu-id="6d5b1-131">是否向收件人发送邮件需要审批。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-131">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="6d5b1-132">例如，如果收件人是大型通讯组列表和审阅者已设置最多批准邮件发送到该通讯组列表，或如果发送给邮件收件人需要审批的收件人的经理。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-132">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="6d5b1-133">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="6d5b1-133">mailboxFull</span></span> | <span data-ttu-id="6d5b1-134">布尔</span><span class="sxs-lookup"><span data-stu-id="6d5b1-134">Boolean</span></span> | <span data-ttu-id="6d5b1-135">收件人邮箱完全状态。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-135">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="6d5b1-136">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="6d5b1-136">maxMessageSize</span></span> | <span data-ttu-id="6d5b1-137">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b1-137">Int32</span></span> | <span data-ttu-id="6d5b1-138">收件人的组织或邮箱已配置最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-138">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="6d5b1-139">recipientScope</span><span class="sxs-lookup"><span data-stu-id="6d5b1-139">recipientScope</span></span> | <span data-ttu-id="6d5b1-140">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="6d5b1-140">recipientScopeType</span></span> | <span data-ttu-id="6d5b1-141">收件人范围。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-141">The scope of the recipient.</span></span> <span data-ttu-id="6d5b1-142">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-142">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="6d5b1-143">例如，管理员可以设置其他组织为其"合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-143">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="6d5b1-144">如果管理员希望某些邮件提示可对特定范围有用范围。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-144">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="6d5b1-145">也很有用，告知人的邮件可能离开组织，以帮助其选择正确决定哪些措词、 语气和内容的发件人。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-145">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="6d5b1-146">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="6d5b1-146">recipientSuggestions</span></span> | <span data-ttu-id="6d5b1-147">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="6d5b1-147">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="6d5b1-148">收件人建议基于以前上下文它们出现在相同的邮件。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-148">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="6d5b1-149">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="6d5b1-149">totalMemberCount</span></span> | <span data-ttu-id="6d5b1-150">Int32</span><span class="sxs-lookup"><span data-stu-id="6d5b1-150">Int32</span></span> | <span data-ttu-id="6d5b1-151">如果收件人是通讯组列表成员的数目。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-151">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="6d5b1-152">recipientScopeType 值</span><span class="sxs-lookup"><span data-stu-id="6d5b1-152">recipientScopeType values</span></span>

| <span data-ttu-id="6d5b1-153">值</span><span class="sxs-lookup"><span data-stu-id="6d5b1-153">Value</span></span>
|:-------------------------
| <span data-ttu-id="6d5b1-154">无</span><span class="sxs-lookup"><span data-stu-id="6d5b1-154">none</span></span>
| <span data-ttu-id="6d5b1-155">内部</span><span class="sxs-lookup"><span data-stu-id="6d5b1-155">internal</span></span>
| <span data-ttu-id="6d5b1-156">外部</span><span class="sxs-lookup"><span data-stu-id="6d5b1-156">external</span></span>
| <span data-ttu-id="6d5b1-157">externalPartner</span><span class="sxs-lookup"><span data-stu-id="6d5b1-157">externalPartner</span></span>
| <span data-ttu-id="6d5b1-158">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="6d5b1-158">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="6d5b1-159">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6d5b1-159">JSON representation</span></span>

<span data-ttu-id="6d5b1-160">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d5b1-160">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "mailtips resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
