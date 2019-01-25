---
title: messageRulePredicates 资源类型
description: 表示适用于某个规则的一组条件和例外情况。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: fda6a160d30dc0d822f2e0aeb5642250d6b69658
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519435"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="01e29-103">messageRulePredicates 资源类型</span><span class="sxs-lookup"><span data-stu-id="01e29-103">messageRulePredicates resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01e29-104">表示适用于某个规则的一组条件和例外情况。</span><span class="sxs-lookup"><span data-stu-id="01e29-104">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="01e29-105">属性</span><span class="sxs-lookup"><span data-stu-id="01e29-105">Properties</span></span>
| <span data-ttu-id="01e29-106">属性</span><span class="sxs-lookup"><span data-stu-id="01e29-106">Property</span></span>     | <span data-ttu-id="01e29-107">类型</span><span class="sxs-lookup"><span data-stu-id="01e29-107">Type</span></span>   |<span data-ttu-id="01e29-108">说明</span><span class="sxs-lookup"><span data-stu-id="01e29-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="01e29-109">bodyContains</span><span class="sxs-lookup"><span data-stu-id="01e29-109">bodyContains</span></span> | <span data-ttu-id="01e29-110">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-110">Collection (String)</span></span> | <span data-ttu-id="01e29-111">表示应该出现在传入邮件正文中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-111">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-112">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="01e29-112">bodyOrSubjectContains</span></span> | <span data-ttu-id="01e29-113">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-113">Collection (String)</span></span> | <span data-ttu-id="01e29-114">表示应该出现在传入邮件正文或主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-114">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-115">categories</span><span class="sxs-lookup"><span data-stu-id="01e29-115">categories</span></span> | <span data-ttu-id="01e29-116">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-116">Collection (String)</span></span> | <span data-ttu-id="01e29-117">表示传入邮件应标记的类别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-117">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-118">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="01e29-118">fromAddresses</span></span> | <span data-ttu-id="01e29-119">Collection ([recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="01e29-119">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="01e29-120">表示传入邮件的特定发件人电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-120">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-121">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="01e29-121">hasAttachments</span></span> | <span data-ttu-id="01e29-122">布尔</span><span class="sxs-lookup"><span data-stu-id="01e29-122">Boolean</span></span> | <span data-ttu-id="01e29-123">指示传入的邮件是否必须包含附件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-123">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-124">headerContains</span><span class="sxs-lookup"><span data-stu-id="01e29-124">headerContains</span></span> | <span data-ttu-id="01e29-125">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-125">Collection (String)</span></span> | <span data-ttu-id="01e29-126">表示出现在传入邮件头中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-126">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-127">importance</span><span class="sxs-lookup"><span data-stu-id="01e29-127">importance</span></span> | <span data-ttu-id="01e29-128">String</span><span class="sxs-lookup"><span data-stu-id="01e29-128">String</span></span> | <span data-ttu-id="01e29-129">传入邮件上标记的重要性，以便条件或例外情况适用：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="01e29-129">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="01e29-130">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="01e29-130">isApprovalRequest</span></span> | <span data-ttu-id="01e29-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-131">Boolean</span></span> | <span data-ttu-id="01e29-132">指示传入的邮件是否必须为审批请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-132">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-133">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="01e29-133">isAutomaticForward</span></span> | <span data-ttu-id="01e29-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-134">Boolean</span></span> | <span data-ttu-id="01e29-135">指示传入的邮件是否必须自动转发，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-135">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-136">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="01e29-136">isAutomaticReply</span></span> | <span data-ttu-id="01e29-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-137">Boolean</span></span> | <span data-ttu-id="01e29-138">指示传入的邮件是否必须自动答复，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-138">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-139">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="01e29-139">isEncrypted</span></span> | <span data-ttu-id="01e29-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-140">Boolean</span></span> | <span data-ttu-id="01e29-141">指示传入的邮件是否必须加密，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-141">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-142">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="01e29-142">isMeetingRequest</span></span> | <span data-ttu-id="01e29-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-143">Boolean</span></span> | <span data-ttu-id="01e29-144">指示传入的邮件是否必须为会议请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-144">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-145">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="01e29-145">isMeetingResponse</span></span> | <span data-ttu-id="01e29-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-146">Boolean</span></span> | <span data-ttu-id="01e29-147">指示传入的邮件是否必须为会议响应，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-147">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-148">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="01e29-148">isNonDeliveryReport</span></span> | <span data-ttu-id="01e29-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-149">Boolean</span></span> | <span data-ttu-id="01e29-150">指示传入的邮件是否必须为未送达报告，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-150">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-151">isPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="01e29-151">isPermissionControlled</span></span> | <span data-ttu-id="01e29-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-152">Boolean</span></span> | <span data-ttu-id="01e29-153">指示传入的邮件是否必须受权限控制（受 RMS 保护），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-153">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-154">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="01e29-154">isReadReceipt</span></span> | <span data-ttu-id="01e29-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-155">Boolean</span></span> | <span data-ttu-id="01e29-156">指示传入的邮件是否必须为已读回执，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-156">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-157">isSigned</span><span class="sxs-lookup"><span data-stu-id="01e29-157">isSigned</span></span> | <span data-ttu-id="01e29-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-158">Boolean</span></span> | <span data-ttu-id="01e29-159">指示传入的邮件是否必须有 S/MIME 签名，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-159">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-160">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="01e29-160">isVoicemail</span></span> | <span data-ttu-id="01e29-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-161">Boolean</span></span> | <span data-ttu-id="01e29-162">指示传入的邮件是否必须有语音邮件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-162">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-163">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="01e29-163">messageActionFlag</span></span> | <span data-ttu-id="01e29-164">String</span><span class="sxs-lookup"><span data-stu-id="01e29-164">String</span></span>  | <span data-ttu-id="01e29-165">表示出现在传入邮件上的 flag-for-action 值，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-165">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="01e29-166">可取值为：`any`、`call`、`doNotForward`、`followUp`、`fyi`、`forward`、`noResponseNecessary`、`read`、`reply`、`replyToAll`、`review`。</span><span class="sxs-lookup"><span data-stu-id="01e29-166">Possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="01e29-167">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="01e29-167">notSentToMe</span></span> | <span data-ttu-id="01e29-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-168">Boolean</span></span> | <span data-ttu-id="01e29-169">指示邮箱所有者是否不能是传入邮件的收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-169">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-170">recipientContains</span><span class="sxs-lookup"><span data-stu-id="01e29-170">recipientContains</span></span> | <span data-ttu-id="01e29-171">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-171">Collection (String)</span></span> | <span data-ttu-id="01e29-172">表示出现在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-172">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-173">senderContains</span><span class="sxs-lookup"><span data-stu-id="01e29-173">senderContains</span></span> | <span data-ttu-id="01e29-174">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-174">Collection (String)</span></span> | <span data-ttu-id="01e29-175">表示出现在传入邮件的 **from** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-175">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-176">sensitivity</span><span class="sxs-lookup"><span data-stu-id="01e29-176">sensitivity</span></span> | <span data-ttu-id="01e29-177">String</span><span class="sxs-lookup"><span data-stu-id="01e29-177">String</span></span> | <span data-ttu-id="01e29-178">表示必须在传入邮件上标记的敏感度级别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-178">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="01e29-179">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="01e29-179">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="01e29-180">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="01e29-180">sentCcMe</span></span> | <span data-ttu-id="01e29-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-181">Boolean</span></span> | <span data-ttu-id="01e29-182">指示邮箱所有者是否必须在传入邮件的 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-182">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-183">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="01e29-183">sentOnlyToMe</span></span> | <span data-ttu-id="01e29-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-184">Boolean</span></span> | <span data-ttu-id="01e29-185">指示邮箱所有者是否必须是传入邮件的唯一收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-185">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-186">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="01e29-186">sentToAddresses</span></span> | <span data-ttu-id="01e29-187">Collection ([recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="01e29-187">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="01e29-188">表示必须已向其发送传入邮件的电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-188">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-189">sentToMe</span><span class="sxs-lookup"><span data-stu-id="01e29-189">sentToMe</span></span> | <span data-ttu-id="01e29-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-190">Boolean</span></span> | <span data-ttu-id="01e29-191">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-191">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-192">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="01e29-192">sentToOrCcMe</span></span> | <span data-ttu-id="01e29-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="01e29-193">Boolean</span></span> | <span data-ttu-id="01e29-194">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-194">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-195">subjectContains</span><span class="sxs-lookup"><span data-stu-id="01e29-195">subjectContains</span></span> | <span data-ttu-id="01e29-196">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="01e29-196">Collection (String)</span></span> | <span data-ttu-id="01e29-197">表示出现在传入邮件主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-197">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="01e29-198">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="01e29-198">withinSizeRange</span></span> | [<span data-ttu-id="01e29-199">sizeRange</span><span class="sxs-lookup"><span data-stu-id="01e29-199">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="01e29-200">表示传入邮件必须介于其中的最小大小和最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="01e29-200">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="01e29-201">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01e29-201">JSON representation</span></span>
<span data-ttu-id="01e29-202">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01e29-202">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "messageRulePredicates resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messagerulepredicates.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
