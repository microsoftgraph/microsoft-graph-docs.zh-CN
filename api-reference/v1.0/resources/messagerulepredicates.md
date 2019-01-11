---
title: messageRulePredicates 资源类型
description: 表示适用于某个规则的一组条件和例外情况。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 13978b4ee09f863ee3f57ac109ee8f3f5adf39c4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804737"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="5f393-103">messageRulePredicates 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f393-103">messageRulePredicates resource type</span></span>


<span data-ttu-id="5f393-104">表示适用于某个规则的一组条件和例外情况。</span><span class="sxs-lookup"><span data-stu-id="5f393-104">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="5f393-105">属性</span><span class="sxs-lookup"><span data-stu-id="5f393-105">Properties</span></span>
| <span data-ttu-id="5f393-106">属性</span><span class="sxs-lookup"><span data-stu-id="5f393-106">Property</span></span>     | <span data-ttu-id="5f393-107">类型</span><span class="sxs-lookup"><span data-stu-id="5f393-107">Type</span></span>   |<span data-ttu-id="5f393-108">说明</span><span class="sxs-lookup"><span data-stu-id="5f393-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5f393-109">bodyContains</span><span class="sxs-lookup"><span data-stu-id="5f393-109">bodyContains</span></span> | <span data-ttu-id="5f393-110">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-110">Collection(String)</span></span> | <span data-ttu-id="5f393-111">表示应该出现在传入邮件正文中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-111">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-112">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="5f393-112">bodyOrSubjectContains</span></span> | <span data-ttu-id="5f393-113">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-113">Collection(String)</span></span> | <span data-ttu-id="5f393-114">表示应该出现在传入邮件正文或主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-114">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-115">categories</span><span class="sxs-lookup"><span data-stu-id="5f393-115">categories</span></span> | <span data-ttu-id="5f393-116">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-116">Collection(String)</span></span> | <span data-ttu-id="5f393-117">表示传入邮件应标记的类别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-117">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-118">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="5f393-118">fromAddresses</span></span> | <span data-ttu-id="5f393-119">集合 （[收件人](recipient.md)）</span><span class="sxs-lookup"><span data-stu-id="5f393-119">Collection([recipient](recipient.md))</span></span> | <span data-ttu-id="5f393-120">表示传入邮件的特定发件人电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-120">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-121">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="5f393-121">hasAttachments</span></span> | <span data-ttu-id="5f393-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-122">Boolean</span></span> | <span data-ttu-id="5f393-123">指示传入的邮件是否必须包含附件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-123">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-124">headerContains</span><span class="sxs-lookup"><span data-stu-id="5f393-124">headerContains</span></span> | <span data-ttu-id="5f393-125">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-125">Collection(String)</span></span> | <span data-ttu-id="5f393-126">表示出现在传入邮件头中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-126">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-127">importance</span><span class="sxs-lookup"><span data-stu-id="5f393-127">importance</span></span> | <span data-ttu-id="5f393-128">importance</span><span class="sxs-lookup"><span data-stu-id="5f393-128">importance</span></span> | <span data-ttu-id="5f393-129">传入邮件上标记的重要性，以便条件或例外情况适用：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="5f393-129">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="5f393-130">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="5f393-130">isApprovalRequest</span></span> | <span data-ttu-id="5f393-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-131">Boolean</span></span> | <span data-ttu-id="5f393-132">指示传入的邮件是否必须为审批请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-132">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-133">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="5f393-133">isAutomaticForward</span></span> | <span data-ttu-id="5f393-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-134">Boolean</span></span> | <span data-ttu-id="5f393-135">指示传入的邮件是否必须自动转发，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-135">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-136">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="5f393-136">isAutomaticReply</span></span> | <span data-ttu-id="5f393-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-137">Boolean</span></span> | <span data-ttu-id="5f393-138">指示传入的邮件是否必须自动答复，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-138">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-139">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="5f393-139">isEncrypted</span></span> | <span data-ttu-id="5f393-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-140">Boolean</span></span> | <span data-ttu-id="5f393-141">指示传入的邮件是否必须加密，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-141">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-142">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5f393-142">isMeetingRequest</span></span> | <span data-ttu-id="5f393-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-143">Boolean</span></span> | <span data-ttu-id="5f393-144">指示传入的邮件是否必须为会议请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-144">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-145">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5f393-145">isMeetingResponse</span></span> | <span data-ttu-id="5f393-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-146">Boolean</span></span> | <span data-ttu-id="5f393-147">指示传入的邮件是否必须为会议响应，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-147">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-148">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="5f393-148">isNonDeliveryReport</span></span> | <span data-ttu-id="5f393-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-149">Boolean</span></span> | <span data-ttu-id="5f393-150">指示传入的邮件是否必须为未送达报告，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-150">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-151">isPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="5f393-151">isPermissionControlled</span></span> | <span data-ttu-id="5f393-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-152">Boolean</span></span> | <span data-ttu-id="5f393-153">指示传入的邮件是否必须受权限控制（受 RMS 保护），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-153">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-154">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="5f393-154">isReadReceipt</span></span> | <span data-ttu-id="5f393-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-155">Boolean</span></span> | <span data-ttu-id="5f393-156">指示传入的邮件是否必须为已读回执，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-156">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-157">isSigned</span><span class="sxs-lookup"><span data-stu-id="5f393-157">isSigned</span></span> | <span data-ttu-id="5f393-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-158">Boolean</span></span> | <span data-ttu-id="5f393-159">指示传入的邮件是否必须有 S/MIME 签名，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-159">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-160">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="5f393-160">isVoicemail</span></span> | <span data-ttu-id="5f393-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-161">Boolean</span></span> | <span data-ttu-id="5f393-162">指示传入的邮件是否必须有语音邮件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-162">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-163">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="5f393-163">messageActionFlag</span></span> | <span data-ttu-id="5f393-164">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="5f393-164">messageActionFlag</span></span>  | <span data-ttu-id="5f393-165">表示出现在传入邮件上的 flag-for-action 值，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-165">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="5f393-166">可能的值为： `any`， `call`， `doNotForward`， `followUp`， `fyi`， `forward`， `noResponseNecessary`， `read`， `reply`， `replyToAll`， `review`。</span><span class="sxs-lookup"><span data-stu-id="5f393-166">The possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="5f393-167">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="5f393-167">notSentToMe</span></span> | <span data-ttu-id="5f393-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-168">Boolean</span></span> | <span data-ttu-id="5f393-169">指示邮箱所有者是否不能是传入邮件的收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-169">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-170">recipientContains</span><span class="sxs-lookup"><span data-stu-id="5f393-170">recipientContains</span></span> | <span data-ttu-id="5f393-171">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-171">Collection(String)</span></span> | <span data-ttu-id="5f393-172">表示出现在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-172">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-173">senderContains</span><span class="sxs-lookup"><span data-stu-id="5f393-173">senderContains</span></span> | <span data-ttu-id="5f393-174">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-174">Collection(String)</span></span> | <span data-ttu-id="5f393-175">表示出现在传入邮件的 **from** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-175">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5f393-176">sensitivity</span></span> | <span data-ttu-id="5f393-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="5f393-177">sensitivity</span></span> | <span data-ttu-id="5f393-178">表示必须在传入邮件上标记的敏感度级别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-178">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="5f393-179">可能的值为： `normal`， `personal`， `private`， `confidential`。</span><span class="sxs-lookup"><span data-stu-id="5f393-179">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="5f393-180">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="5f393-180">sentCcMe</span></span> | <span data-ttu-id="5f393-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-181">Boolean</span></span> | <span data-ttu-id="5f393-182">指示邮箱所有者是否必须在传入邮件的 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-182">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-183">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="5f393-183">sentOnlyToMe</span></span> | <span data-ttu-id="5f393-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-184">Boolean</span></span> | <span data-ttu-id="5f393-185">指示邮箱所有者是否必须是传入邮件的唯一收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-185">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-186">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="5f393-186">sentToAddresses</span></span> | <span data-ttu-id="5f393-187">集合 （[收件人](recipient.md)）</span><span class="sxs-lookup"><span data-stu-id="5f393-187">Collection([recipient](recipient.md))</span></span> | <span data-ttu-id="5f393-188">表示必须已向其发送传入邮件的电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-188">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-189">sentToMe</span><span class="sxs-lookup"><span data-stu-id="5f393-189">sentToMe</span></span> | <span data-ttu-id="5f393-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-190">Boolean</span></span> | <span data-ttu-id="5f393-191">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-191">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-192">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="5f393-192">sentToOrCcMe</span></span> | <span data-ttu-id="5f393-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="5f393-193">Boolean</span></span> | <span data-ttu-id="5f393-194">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-194">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-195">subjectContains</span><span class="sxs-lookup"><span data-stu-id="5f393-195">subjectContains</span></span> | <span data-ttu-id="5f393-196">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="5f393-196">Collection(String)</span></span> | <span data-ttu-id="5f393-197">表示出现在传入邮件主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-197">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="5f393-198">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="5f393-198">withinSizeRange</span></span> | [<span data-ttu-id="5f393-199">sizeRange</span><span class="sxs-lookup"><span data-stu-id="5f393-199">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="5f393-200">表示传入邮件必须介于其中的最小大小和最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="5f393-200">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5f393-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f393-201">JSON representation</span></span>
<span data-ttu-id="5f393-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f393-202">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRulePredicates"
}-->

```json
{
  "bodyContains": ["String"],
  "bodyOrSubjectContains": ["String"],
  "categories": ["String"],
  "fromAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "hasAttachments": "Boolean",
  "headerContains": ["String"],
  "importance": "String",
  "isApprovalRequest": "Boolean",
  "isAutomaticForward": "Boolean",
  "isAutomaticReply": "Boolean",
  "isEncrypted": "Boolean",
  "isMeetingRequest": "Boolean",
  "isMeetingResponse": "Boolean",
  "isNonDeliveryReport": "Boolean",
  "isPermissionControlled": "Boolean",
  "isReadReceipt": "Boolean",
  "isSigned": "Boolean",
  "isVoicemail": "Boolean",
  "messageActionFlag": "String",
  "notSentToMe": "Boolean",
  "recipientContains": ["String"],
  "senderContains": ["String"],
  "sensitivity": "String",
  "sentCcMe": "Boolean",
  "sentOnlyToMe": "Boolean",
  "sentToAddresses": [{"@odata.type": "microsoft.graph.recipient"}],
  "sentToMe": "Boolean",
  "sentToOrCcMe": "Boolean",
  "subjectContains": ["String"],
  "withinSizeRange": {"@odata.type": "microsoft.graph.sizeRange"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
