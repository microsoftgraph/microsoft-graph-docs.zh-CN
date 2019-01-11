---
title: 邮件提示资源类型
description: '有关提示性消息收件人，它们撰写邮件时向用户显示。 例如，-外出消息 '
localization_priority: Normal
ms.openlocfilehash: 62955594412b2d42a4d05b4b13858c4e511605df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27860639"
---
# <a name="mailtips-resource-type"></a><span data-ttu-id="0a7ea-104">邮件提示资源类型</span><span class="sxs-lookup"><span data-stu-id="0a7ea-104">mailTips resource type</span></span>

> <span data-ttu-id="0a7ea-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a7ea-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0a7ea-107">有关提示性消息收件人，它们撰写邮件时向用户显示。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-107">Informative messages about a recipient, that are displayed to users while they are composing a message.</span></span> <span data-ttu-id="0a7ea-108">例如，作为自动回复邮件收件人-外出邮件。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-108">For example, an out-of-office message as an automatic reply for a message recipient.</span></span>


## <a name="properties"></a><span data-ttu-id="0a7ea-109">属性</span><span class="sxs-lookup"><span data-stu-id="0a7ea-109">Properties</span></span>
| <span data-ttu-id="0a7ea-110">属性</span><span class="sxs-lookup"><span data-stu-id="0a7ea-110">Property</span></span>     | <span data-ttu-id="0a7ea-111">类型</span><span class="sxs-lookup"><span data-stu-id="0a7ea-111">Type</span></span>   |<span data-ttu-id="0a7ea-112">Description</span><span class="sxs-lookup"><span data-stu-id="0a7ea-112">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0a7ea-113">automaticReplies</span><span class="sxs-lookup"><span data-stu-id="0a7ea-113">automaticReplies</span></span> | [<span data-ttu-id="0a7ea-114">automaticRepliesMailTips</span><span class="sxs-lookup"><span data-stu-id="0a7ea-114">automaticRepliesMailTips</span></span>](../resources/automaticrepliesmailtips.md) | <span data-ttu-id="0a7ea-115">如果已被收件人设置，邮件自动回复的提示。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-115">Mail tips for automatic reply if it has been set up by the recipient.</span></span> |
| <span data-ttu-id="0a7ea-116">customMailTip</span><span class="sxs-lookup"><span data-stu-id="0a7ea-116">customMailTip</span></span> | <span data-ttu-id="0a7ea-117">字符串</span><span class="sxs-lookup"><span data-stu-id="0a7ea-117">String</span></span> | <span data-ttu-id="0a7ea-118">可在收件人的邮箱中设置自定义邮件提示。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-118">A custom mail tip that can be set on the recipient's mailbox.</span></span> |
| <span data-ttu-id="0a7ea-119">deliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="0a7ea-119">deliveryRestricted</span></span>| <span data-ttu-id="0a7ea-120">布尔</span><span class="sxs-lookup"><span data-stu-id="0a7ea-120">Boolean</span></span> | <span data-ttu-id="0a7ea-121">收件人的邮箱是否受限制，例如，接受从预定义列表的发件人的邮件拒绝来自发件人的预定义列表的邮件，或接受来自仅经过身份验证发件人的邮件。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-121">Whether the recipient's mailbox is restricted, for example, accepting messages from only a predefined list of senders, rejecting messages from a predefined list of senders, or accepting messages from only authenticated senders.</span></span> |
| <span data-ttu-id="0a7ea-122">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a7ea-122">emailAddress</span></span> | [<span data-ttu-id="0a7ea-123">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0a7ea-123">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="0a7ea-124">若要获取的邮件提示收件人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-124">The email address of the recipient to get mailtips for.</span></span> |
| <span data-ttu-id="0a7ea-125">error</span><span class="sxs-lookup"><span data-stu-id="0a7ea-125">error</span></span> | [<span data-ttu-id="0a7ea-126">mailTipsError</span><span class="sxs-lookup"><span data-stu-id="0a7ea-126">mailTipsError</span></span>](../resources/mailtipserror.md) | <span data-ttu-id="0a7ea-127">在[getMailTips](../api/user-getmailtips.md)操作过程中出现错误。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-127">Errors that occur during the [getMailTips](../api/user-getmailtips.md) action.</span></span> |
| <span data-ttu-id="0a7ea-128">externalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0a7ea-128">externalMemberCount</span></span> | <span data-ttu-id="0a7ea-129">Int32</span><span class="sxs-lookup"><span data-stu-id="0a7ea-129">Int32</span></span> | <span data-ttu-id="0a7ea-130">如果收件人是通讯组列表的外部成员的数目。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-130">The number of external members if the recipient is a distribution list.</span></span> |
| <span data-ttu-id="0a7ea-131">isModerated</span><span class="sxs-lookup"><span data-stu-id="0a7ea-131">isModerated</span></span> |<span data-ttu-id="0a7ea-132">布尔</span><span class="sxs-lookup"><span data-stu-id="0a7ea-132">Boolean</span></span>  | <span data-ttu-id="0a7ea-133">是否向收件人发送邮件需要审批。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-133">Whether sending messages to the recipient requires approval.</span></span> <span data-ttu-id="0a7ea-134">例如，如果收件人是大型通讯组列表和审阅者已设置最多批准邮件发送到该通讯组列表，或如果发送给邮件收件人需要审批的收件人的经理。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-134">For example, if the recipient is a large distribution list and a moderator has been set up to approve messages sent to that distribution list, or if sending messages to a recipient requires approval of the recipient's manager.</span></span> |
| <span data-ttu-id="0a7ea-135">mailboxFull</span><span class="sxs-lookup"><span data-stu-id="0a7ea-135">mailboxFull</span></span> | <span data-ttu-id="0a7ea-136">布尔</span><span class="sxs-lookup"><span data-stu-id="0a7ea-136">Boolean</span></span> | <span data-ttu-id="0a7ea-137">收件人邮箱完全状态。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-137">The mailbox full status of the recipient.</span></span> |
| <span data-ttu-id="0a7ea-138">maxMessageSize</span><span class="sxs-lookup"><span data-stu-id="0a7ea-138">maxMessageSize</span></span> | <span data-ttu-id="0a7ea-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0a7ea-139">Int32</span></span> | <span data-ttu-id="0a7ea-140">收件人的组织或邮箱已配置最大邮件大小。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-140">The maximum message size that has been configured for the recipient's organization or mailbox.</span></span> |
| <span data-ttu-id="0a7ea-141">recipientScope</span><span class="sxs-lookup"><span data-stu-id="0a7ea-141">recipientScope</span></span> | <span data-ttu-id="0a7ea-142">字符串</span><span class="sxs-lookup"><span data-stu-id="0a7ea-142">String</span></span> | <span data-ttu-id="0a7ea-143">收件人范围。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-143">The scope of the recipient.</span></span> <span data-ttu-id="0a7ea-144">可取值为：`none`、`internal`、`external`、`externalPartner`、`externalNonParther`。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-144">Possible values are: `none`, `internal`, `external`, `externalPartner`, `externalNonParther`.</span></span> <span data-ttu-id="0a7ea-145">例如，管理员可以设置其他组织为其"合作伙伴"。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-145">For example, an administrator can set another organization to be its "partner".</span></span> <span data-ttu-id="0a7ea-146">如果管理员希望某些邮件提示可对特定范围有用范围。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-146">The scope is useful if an administrator wants certain mailtips to be accessible to certain scopes.</span></span> <span data-ttu-id="0a7ea-147">也很有用，告知人的邮件可能离开组织，以帮助其选择正确决定哪些措词、 语气和内容的发件人。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-147">It's also useful to senders to inform them that their message may leave the organization, helping them make the correct decisions about wording, tone and content.</span></span>|
| <span data-ttu-id="0a7ea-148">recipientSuggestions</span><span class="sxs-lookup"><span data-stu-id="0a7ea-148">recipientSuggestions</span></span> | <span data-ttu-id="0a7ea-149">[recipient](../resources/recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="0a7ea-149">[recipient](../resources/recipient.md) collection</span></span> | <span data-ttu-id="0a7ea-150">收件人建议基于以前上下文它们出现在相同的邮件。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-150">Recipients suggested based on previous contexts where they appear in the same message.</span></span> |
| <span data-ttu-id="0a7ea-151">totalMemberCount</span><span class="sxs-lookup"><span data-stu-id="0a7ea-151">totalMemberCount</span></span> | <span data-ttu-id="0a7ea-152">Int32</span><span class="sxs-lookup"><span data-stu-id="0a7ea-152">Int32</span></span> | <span data-ttu-id="0a7ea-153">如果收件人是通讯组列表成员的数目。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-153">The number of members if the recipient is a distribution list.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="0a7ea-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0a7ea-154">JSON representation</span></span>

<span data-ttu-id="0a7ea-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0a7ea-155">Here is a JSON representation of the resource.</span></span>

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
