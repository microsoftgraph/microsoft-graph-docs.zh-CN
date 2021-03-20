---
title: 邮件提示资源类型
description: '有关收件人的信息性消息，在用户撰写邮件时向用户显示。 例如，外出邮件 '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 0a2dfe421c19b49c8c7f489bef55890a058e2c40
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941370"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="0d6d9-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="0d6d9-104">mailTips resource type</span></span>

<span data-ttu-id="0d6d9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d6d9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0d6d9-106">有关收件人的信息性消息，在用户撰写邮件时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="0d6d9-107">例如，外出邮件作为邮件收件人的自动答复。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="0d6d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d6d9-108">Properties</span></span>
| <span data-ttu-id="0d6d9-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d6d9-109">Property</span></span>     | <span data-ttu-id="0d6d9-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d6d9-110">Type</span></span>   |<span data-ttu-id="0d6d9-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d6d9-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0d6d9-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="0d6d9-112">automaticReplies</span></span> | [<span data-ttu-id="0d6d9-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="0d6d9-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="0d6d9-114">自动答复的邮件提示（如果收件人已设置）。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="0d6d9-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="0d6d9-115">customMailTip</span></span> | <span data-ttu-id="0d6d9-116">String</span><span class="sxs-lookup"><span data-stu-id="0d6d9-116">String</span></span> | <span data-ttu-id="0d6d9-117">可以在收件人邮箱上设置的自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="0d6d9-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="0d6d9-118">deliveryRestricted</span></span>| <span data-ttu-id="0d6d9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d6d9-119">Boolean</span></span> | <span data-ttu-id="0d6d9-120">例如，是否限制收件人的邮箱，例如仅接受来自预定义发件人列表的邮件、拒绝来自预定义发件人列表的邮件或仅接受来自经过身份验证的发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="0d6d9-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d6d9-121">emailAddress</span></span> | [<span data-ttu-id="0d6d9-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0d6d9-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="0d6d9-123">要获取其邮件提示的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="0d6d9-124">error</span><span class="sxs-lookup"><span data-stu-id="0d6d9-124">error</span></span> | [<span data-ttu-id="0d6d9-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="0d6d9-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="0d6d9-126">[getMailTips 操作期间发生的](../api/user-getmailtips.md)错误。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="0d6d9-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0d6d9-127">externalMemberCount</span></span> | <span data-ttu-id="0d6d9-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0d6d9-128">Int32</span></span> | <span data-ttu-id="0d6d9-129">如果收件人是通讯组列表，则外部成员的数量。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="0d6d9-130">isModerated</span><span class="sxs-lookup"><span data-stu-id="0d6d9-130">isModerated</span></span> |<span data-ttu-id="0d6d9-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d6d9-131">Boolean</span></span>  | <span data-ttu-id="0d6d9-132">是否向收件人发送邮件需要审批。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="0d6d9-133">例如，如果收件人是一个大型通讯组列表，并且已设置仲裁人来批准发送到该通讯组列表的邮件，或者向收件人发送邮件需要收件人的经理批准。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="0d6d9-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="0d6d9-134">mailboxFull</span></span> | <span data-ttu-id="0d6d9-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d6d9-135">Boolean</span></span> | <span data-ttu-id="0d6d9-136">收件人的邮箱完整状态。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="0d6d9-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="0d6d9-137">maxMessageSize</span></span> | <span data-ttu-id="0d6d9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="0d6d9-138">Int32</span></span> | <span data-ttu-id="0d6d9-139">为收件人的组织或邮箱配置的最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="0d6d9-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="0d6d9-140">recipientScope</span></span> | <span data-ttu-id="0d6d9-141">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="0d6d9-141">recipientScopeType</span></span> | <span data-ttu-id="0d6d9-142">收件人的作用域。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-142">The scope of the recipient.</span></span> <span data-ttu-id="0d6d9-143">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="0d6d9-144">例如，管理员可以将另一个组织设置为其"合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="0d6d9-145">如果管理员希望某些邮件提示可供某些作用域访问，则范围非常有用。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="0d6d9-146">发件人还可以通知他们其邮件可能离开组织，帮助他们做出有关语气、语气和内容的正确决策。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="0d6d9-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="0d6d9-147">recipientSuggestions</span></span> | <span data-ttu-id="0d6d9-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="0d6d9-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="0d6d9-149">基于之前在同一邮件中的显示上下文建议的收件人。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="0d6d9-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0d6d9-150">totalMemberCount</span></span> | <span data-ttu-id="0d6d9-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0d6d9-151">Int32</span></span> | <span data-ttu-id="0d6d9-152">如果收件人是通讯组列表，则成员数。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-152">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0d6d9-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d6d9-153">JSON representation</span></span>

<span data-ttu-id="0d6d9-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d6d9-154">Here is a JSON representation of the resource.</span></span>

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

