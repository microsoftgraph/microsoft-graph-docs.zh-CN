---
title: messageRulePredicates 资源类型
description: 表示适用于某个规则的一组条件和例外情况。
ms.openlocfilehash: 068f90b6557021c6c77b11cfe0851255dd427ea3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043009"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="db9e0-103">messageRulePredicates 资源类型</span><span class="sxs-lookup"><span data-stu-id="db9e0-103">messageRulePredicates resource type</span></span>

> <span data-ttu-id="db9e0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="db9e0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="db9e0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="db9e0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="db9e0-106">表示适用于某个规则的一组条件和例外情况。</span><span class="sxs-lookup"><span data-stu-id="db9e0-106">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="db9e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="db9e0-107">Properties</span></span>
| <span data-ttu-id="db9e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="db9e0-108">Property</span></span>     | <span data-ttu-id="db9e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="db9e0-109">Type</span></span>   |<span data-ttu-id="db9e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="db9e0-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="db9e0-111">bodyContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-111">bodyContains</span></span> | <span data-ttu-id="db9e0-112">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-112">Collection (String)</span></span> | <span data-ttu-id="db9e0-113">表示应该出现在传入邮件正文中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-113">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-114">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-114">bodyOrSubjectContains</span></span> | <span data-ttu-id="db9e0-115">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-115">Collection (String)</span></span> | <span data-ttu-id="db9e0-116">表示应该出现在传入邮件正文或主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-116">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-117">categories</span><span class="sxs-lookup"><span data-stu-id="db9e0-117">categories</span></span> | <span data-ttu-id="db9e0-118">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-118">Collection (String)</span></span> | <span data-ttu-id="db9e0-119">表示传入邮件应标记的类别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-119">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-120">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="db9e0-120">fromAddresses</span></span> | <span data-ttu-id="db9e0-121">Collection ([recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="db9e0-121">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="db9e0-122">表示传入邮件的特定发件人电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-122">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-123">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="db9e0-123">hasAttachments</span></span> | <span data-ttu-id="db9e0-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-124">Boolean</span></span> | <span data-ttu-id="db9e0-125">指示传入的邮件是否必须包含附件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-125">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-126">headerContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-126">headerContains</span></span> | <span data-ttu-id="db9e0-127">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-127">Collection (String)</span></span> | <span data-ttu-id="db9e0-128">表示出现在传入邮件头中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-128">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-129">importance</span><span class="sxs-lookup"><span data-stu-id="db9e0-129">importance</span></span> | <span data-ttu-id="db9e0-130">String</span><span class="sxs-lookup"><span data-stu-id="db9e0-130">String</span></span> | <span data-ttu-id="db9e0-131">传入邮件上标记的重要性，以便条件或例外情况适用：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="db9e0-131">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="db9e0-132">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="db9e0-132">isApprovalRequest</span></span> | <span data-ttu-id="db9e0-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-133">Boolean</span></span> | <span data-ttu-id="db9e0-134">指示传入的邮件是否必须为审批请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-134">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-135">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="db9e0-135">isAutomaticForward</span></span> | <span data-ttu-id="db9e0-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-136">Boolean</span></span> | <span data-ttu-id="db9e0-137">指示传入的邮件是否必须自动转发，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-137">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-138">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="db9e0-138">isAutomaticReply</span></span> | <span data-ttu-id="db9e0-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-139">Boolean</span></span> | <span data-ttu-id="db9e0-140">指示传入的邮件是否必须自动答复，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-140">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-141">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="db9e0-141">isEncrypted</span></span> | <span data-ttu-id="db9e0-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-142">Boolean</span></span> | <span data-ttu-id="db9e0-143">指示传入的邮件是否必须加密，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-143">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-144">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="db9e0-144">isMeetingRequest</span></span> | <span data-ttu-id="db9e0-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-145">Boolean</span></span> | <span data-ttu-id="db9e0-146">指示传入的邮件是否必须为会议请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-146">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-147">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="db9e0-147">isMeetingResponse</span></span> | <span data-ttu-id="db9e0-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-148">Boolean</span></span> | <span data-ttu-id="db9e0-149">指示传入的邮件是否必须为会议响应，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-149">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-150">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="db9e0-150">isNonDeliveryReport</span></span> | <span data-ttu-id="db9e0-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-151">Boolean</span></span> | <span data-ttu-id="db9e0-152">指示传入的邮件是否必须为未送达报告，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-152">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-153">isPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="db9e0-153">isPermissionControlled</span></span> | <span data-ttu-id="db9e0-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-154">Boolean</span></span> | <span data-ttu-id="db9e0-155">指示传入的邮件是否必须受权限控制（受 RMS 保护），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-155">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-156">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="db9e0-156">isReadReceipt</span></span> | <span data-ttu-id="db9e0-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-157">Boolean</span></span> | <span data-ttu-id="db9e0-158">指示传入的邮件是否必须为已读回执，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-158">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-159">isSigned</span><span class="sxs-lookup"><span data-stu-id="db9e0-159">isSigned</span></span> | <span data-ttu-id="db9e0-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-160">Boolean</span></span> | <span data-ttu-id="db9e0-161">指示传入的邮件是否必须有 S/MIME 签名，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-161">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-162">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="db9e0-162">isVoicemail</span></span> | <span data-ttu-id="db9e0-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-163">Boolean</span></span> | <span data-ttu-id="db9e0-164">指示传入的邮件是否必须有语音邮件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-164">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-165">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="db9e0-165">messageActionFlag</span></span> | <span data-ttu-id="db9e0-166">String</span><span class="sxs-lookup"><span data-stu-id="db9e0-166">String</span></span>  | <span data-ttu-id="db9e0-167">表示出现在传入邮件上的 flag-for-action 值，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-167">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="db9e0-168">可取值为：`any`、`call`、`doNotForward`、`followUp`、`fyi`、`forward`、`noResponseNecessary`、`read`、`reply`、`replyToAll`、`review`。</span><span class="sxs-lookup"><span data-stu-id="db9e0-168">Possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="db9e0-169">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="db9e0-169">notSentToMe</span></span> | <span data-ttu-id="db9e0-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-170">Boolean</span></span> | <span data-ttu-id="db9e0-171">指示邮箱所有者是否不能是传入邮件的收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-171">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-172">recipientContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-172">recipientContains</span></span> | <span data-ttu-id="db9e0-173">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-173">Collection (String)</span></span> | <span data-ttu-id="db9e0-174">表示出现在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-174">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-175">senderContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-175">senderContains</span></span> | <span data-ttu-id="db9e0-176">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-176">Collection (String)</span></span> | <span data-ttu-id="db9e0-177">表示出现在传入邮件的 **from** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-177">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-178">sensitivity</span><span class="sxs-lookup"><span data-stu-id="db9e0-178">sensitivity</span></span> | <span data-ttu-id="db9e0-179">String</span><span class="sxs-lookup"><span data-stu-id="db9e0-179">String</span></span> | <span data-ttu-id="db9e0-180">表示必须在传入邮件上标记的敏感度级别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-180">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="db9e0-181">可取值为：`normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="db9e0-181">Possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="db9e0-182">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="db9e0-182">sentCcMe</span></span> | <span data-ttu-id="db9e0-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-183">Boolean</span></span> | <span data-ttu-id="db9e0-184">指示邮箱所有者是否必须在传入邮件的 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-184">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-185">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="db9e0-185">sentOnlyToMe</span></span> | <span data-ttu-id="db9e0-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-186">Boolean</span></span> | <span data-ttu-id="db9e0-187">指示邮箱所有者是否必须是传入邮件的唯一收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-187">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-188">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="db9e0-188">sentToAddresses</span></span> | <span data-ttu-id="db9e0-189">Collection ([recipient](recipient.md))</span><span class="sxs-lookup"><span data-stu-id="db9e0-189">Collection ([recipient](recipient.md))</span></span> | <span data-ttu-id="db9e0-190">表示必须已向其发送传入邮件的电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-190">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-191">sentToMe</span><span class="sxs-lookup"><span data-stu-id="db9e0-191">sentToMe</span></span> | <span data-ttu-id="db9e0-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-192">Boolean</span></span> | <span data-ttu-id="db9e0-193">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-193">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-194">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="db9e0-194">sentToOrCcMe</span></span> | <span data-ttu-id="db9e0-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="db9e0-195">Boolean</span></span> | <span data-ttu-id="db9e0-196">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-196">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-197">subjectContains</span><span class="sxs-lookup"><span data-stu-id="db9e0-197">subjectContains</span></span> | <span data-ttu-id="db9e0-198">Collection (String)</span><span class="sxs-lookup"><span data-stu-id="db9e0-198">Collection (String)</span></span> | <span data-ttu-id="db9e0-199">表示出现在传入邮件主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-199">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="db9e0-200">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="db9e0-200">withinSizeRange</span></span> | [<span data-ttu-id="db9e0-201">sizeRange</span><span class="sxs-lookup"><span data-stu-id="db9e0-201">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="db9e0-202">表示传入邮件必须介于其中的最小大小和最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="db9e0-202">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |



## <a name="json-representation"></a><span data-ttu-id="db9e0-203">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db9e0-203">JSON representation</span></span>
<span data-ttu-id="db9e0-204">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db9e0-204">Here is a JSON representation of the resource.</span></span>

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