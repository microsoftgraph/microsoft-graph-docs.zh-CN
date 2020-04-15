---
title: 邮件提示资源类型
description: '有关收件人的信息性消息，在用户撰写邮件时向其显示。 例如，外出邮件 '
localization_priority: Normal
author: svpsiva
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 926f2c48981da637083e747245ecdee1b94351cb
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43461836"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="d00fc-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="d00fc-104">mailTips resource type</span></span>

<span data-ttu-id="d00fc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d00fc-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d00fc-106">有关收件人的信息性消息，在用户撰写邮件时向其显示。</span><span class="sxs-lookup"><span data-stu-id="d00fc-106">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="d00fc-107">例如，外出邮件作为邮件收件人的自动答复。</span><span class="sxs-lookup"><span data-stu-id="d00fc-107">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="d00fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d00fc-108">Properties</span></span>
| <span data-ttu-id="d00fc-109">属性</span><span class="sxs-lookup"><span data-stu-id="d00fc-109">Property</span></span>     | <span data-ttu-id="d00fc-110">类型</span><span class="sxs-lookup"><span data-stu-id="d00fc-110">Type</span></span>   |<span data-ttu-id="d00fc-111">说明</span><span class="sxs-lookup"><span data-stu-id="d00fc-111">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d00fc-112">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="d00fc-112">automaticReplies</span></span> | [<span data-ttu-id="d00fc-113">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="d00fc-113">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="d00fc-114">"自动答复" 的邮件提示（如果收件人已设置）。</span><span class="sxs-lookup"><span data-stu-id="d00fc-114">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="d00fc-115">customMailTip</span><span class="sxs-lookup"><span data-stu-id="d00fc-115">customMailTip</span></span> | <span data-ttu-id="d00fc-116">String</span><span class="sxs-lookup"><span data-stu-id="d00fc-116">String</span></span> | <span data-ttu-id="d00fc-117">可在收件人邮箱上设置的自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="d00fc-117">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="d00fc-118">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="d00fc-118">deliveryRestricted</span></span>| <span data-ttu-id="d00fc-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d00fc-119">Boolean</span></span> | <span data-ttu-id="d00fc-120">收件人邮箱是否受到限制，例如，仅接受来自预定义的发件人列表的邮件、拒绝来自预定义的发件人列表的邮件，还是仅接受来自已验证的发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="d00fc-120">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="d00fc-121">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d00fc-121">emailAddress</span></span> | [<span data-ttu-id="d00fc-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d00fc-122">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="d00fc-123">要获取其邮件提示的收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="d00fc-123">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="d00fc-124">error</span><span class="sxs-lookup"><span data-stu-id="d00fc-124">error</span></span> | [<span data-ttu-id="d00fc-125">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="d00fc-125">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="d00fc-126">[GetMailTips](../api/user-getmailtips.md)操作过程中发生的错误。</span><span class="sxs-lookup"><span data-stu-id="d00fc-126">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="d00fc-127">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d00fc-127">externalMemberCount</span></span> | <span data-ttu-id="d00fc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d00fc-128">Int32</span></span> | <span data-ttu-id="d00fc-129">如果收件人是通讯组列表，则为外部成员的数量。</span><span class="sxs-lookup"><span data-stu-id="d00fc-129">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="d00fc-130">isModerated</span><span class="sxs-lookup"><span data-stu-id="d00fc-130">isModerated</span></span> |<span data-ttu-id="d00fc-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d00fc-131">Boolean</span></span>  | <span data-ttu-id="d00fc-132">向收件人发送邮件是否需要审批。</span><span class="sxs-lookup"><span data-stu-id="d00fc-132">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="d00fc-133">例如，如果收件人是一个大型通讯组列表，并且已将仲裁人设置为审批发送到该通讯组列表的邮件，或者向收件人发送邮件时需要对收件人的经理进行审批。</span><span class="sxs-lookup"><span data-stu-id="d00fc-133">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="d00fc-134">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="d00fc-134">mailboxFull</span></span> | <span data-ttu-id="d00fc-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d00fc-135">Boolean</span></span> | <span data-ttu-id="d00fc-136">收件人的邮箱完整状态。</span><span class="sxs-lookup"><span data-stu-id="d00fc-136">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="d00fc-137">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="d00fc-137">maxMessageSize</span></span> | <span data-ttu-id="d00fc-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d00fc-138">Int32</span></span> | <span data-ttu-id="d00fc-139">已为收件人的组织或邮箱配置的最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="d00fc-139">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="d00fc-140">recipientScope</span><span class="sxs-lookup"><span data-stu-id="d00fc-140">recipientScope</span></span> | <span data-ttu-id="d00fc-141">recipientScopeType</span><span class="sxs-lookup"><span data-stu-id="d00fc-141">recipientScopeType</span></span> | <span data-ttu-id="d00fc-142">收件人的范围。</span><span class="sxs-lookup"><span data-stu-id="d00fc-142">The scope of the recipient.</span></span> <span data-ttu-id="d00fc-143">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="d00fc-143">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="d00fc-144">例如，管理员可以将其他组织设置为其 "合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="d00fc-144">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="d00fc-145">如果管理员希望某些范围能够访问某些邮件提示，则该范围很有用。</span><span class="sxs-lookup"><span data-stu-id="d00fc-145">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="d00fc-146">对于发件人来说，通知他们其邮件可能会离开组织，从而帮助他们做出正确的措辞、语气和内容决策。</span><span class="sxs-lookup"><span data-stu-id="d00fc-146">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="d00fc-147">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="d00fc-147">recipientSuggestions</span></span> | <span data-ttu-id="d00fc-148">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="d00fc-148">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="d00fc-149">根据以前的上下文显示在同一邮件中建议的收件人。</span><span class="sxs-lookup"><span data-stu-id="d00fc-149">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="d00fc-150">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="d00fc-150">totalMemberCount</span></span> | <span data-ttu-id="d00fc-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d00fc-151">Int32</span></span> | <span data-ttu-id="d00fc-152">如果收件人是通讯组列表，则为成员数量。</span><span class="sxs-lookup"><span data-stu-id="d00fc-152">The number of members if the recipient is a distribution list.</span></span> |

### <a name="recipientscopetype-values"></a><span data-ttu-id="d00fc-153">recipientScopeType 值</span><span class="sxs-lookup"><span data-stu-id="d00fc-153">recipientScopeType values</span></span>

| <span data-ttu-id="d00fc-154">值</span><span class="sxs-lookup"><span data-stu-id="d00fc-154">Value</span></span>
|:-------------------------
| <span data-ttu-id="d00fc-155">无</span><span class="sxs-lookup"><span data-stu-id="d00fc-155">none</span></span>
| <span data-ttu-id="d00fc-156">里面</span><span class="sxs-lookup"><span data-stu-id="d00fc-156">internal</span></span>
| <span data-ttu-id="d00fc-157">对外</span><span class="sxs-lookup"><span data-stu-id="d00fc-157">external</span></span>
| <span data-ttu-id="d00fc-158">externalPartner</span><span class="sxs-lookup"><span data-stu-id="d00fc-158">externalPartner</span></span>
| <span data-ttu-id="d00fc-159">externalNonPartner</span><span class="sxs-lookup"><span data-stu-id="d00fc-159">externalNonPartner</span></span>


## <a name="json-representation"></a><span data-ttu-id="d00fc-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d00fc-160">JSON representation</span></span>

<span data-ttu-id="d00fc-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d00fc-161">Here is a JSON representation of the resource.</span></span>

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
