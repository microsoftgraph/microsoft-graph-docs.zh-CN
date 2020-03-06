---
title: messageRulePredicates 资源类型
description: 表示适用于某个规则的一组条件和例外情况。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d40763e53aef06209818476314bca76ad2ba1293
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42534235"
---
# <a name="messagerulepredicates-resource-type"></a><span data-ttu-id="89843-103">messageRulePredicates 资源类型</span><span class="sxs-lookup"><span data-stu-id="89843-103">messageRulePredicates resource type</span></span>

<span data-ttu-id="89843-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89843-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="89843-105">表示适用于某个规则的一组条件和例外情况。</span><span class="sxs-lookup"><span data-stu-id="89843-105">Represents the set of conditions and exceptions that are available for a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="89843-106">属性</span><span class="sxs-lookup"><span data-stu-id="89843-106">Properties</span></span>
| <span data-ttu-id="89843-107">属性</span><span class="sxs-lookup"><span data-stu-id="89843-107">Property</span></span>     | <span data-ttu-id="89843-108">类型</span><span class="sxs-lookup"><span data-stu-id="89843-108">Type</span></span>   |<span data-ttu-id="89843-109">说明</span><span class="sxs-lookup"><span data-stu-id="89843-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="89843-110">bodyContains</span><span class="sxs-lookup"><span data-stu-id="89843-110">bodyContains</span></span> | <span data-ttu-id="89843-111">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-111">Collection(String)</span></span> | <span data-ttu-id="89843-112">表示应该出现在传入邮件正文中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-112">Represents the strings that should appear in the body of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-113">bodyOrSubjectContains</span><span class="sxs-lookup"><span data-stu-id="89843-113">bodyOrSubjectContains</span></span> | <span data-ttu-id="89843-114">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-114">Collection(String)</span></span> | <span data-ttu-id="89843-115">表示应该出现在传入邮件正文或主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-115">Represents the strings that should appear in the body or subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-116">categories</span><span class="sxs-lookup"><span data-stu-id="89843-116">categories</span></span> | <span data-ttu-id="89843-117">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-117">Collection(String)</span></span> | <span data-ttu-id="89843-118">表示传入邮件应标记的类别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-118">Represents the categories that an incoming message should be labeled with in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-119">fromAddresses</span><span class="sxs-lookup"><span data-stu-id="89843-119">fromAddresses</span></span> | <span data-ttu-id="89843-120">集合（[收件人](recipient.md)）</span><span class="sxs-lookup"><span data-stu-id="89843-120">Collection([recipient](recipient.md))</span></span> | <span data-ttu-id="89843-121">表示传入邮件的特定发件人电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-121">Represents the specific sender email addresses of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-122">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="89843-122">hasAttachments</span></span> | <span data-ttu-id="89843-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-123">Boolean</span></span> | <span data-ttu-id="89843-124">指示传入的邮件是否必须包含附件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-124">Indicates whether an incoming message must have attachments in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-125">headerContains</span><span class="sxs-lookup"><span data-stu-id="89843-125">headerContains</span></span> | <span data-ttu-id="89843-126">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-126">Collection(String)</span></span> | <span data-ttu-id="89843-127">表示出现在传入邮件头中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-127">Represents the strings that appear in the headers of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-128">importance</span><span class="sxs-lookup"><span data-stu-id="89843-128">importance</span></span> | <span data-ttu-id="89843-129">importance</span><span class="sxs-lookup"><span data-stu-id="89843-129">importance</span></span> | <span data-ttu-id="89843-130">传入邮件上标记的重要性，以便条件或例外情况适用：`low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="89843-130">The importance that is stamped on an incoming message in order for the condition or exception to apply: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="89843-131">isApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="89843-131">isApprovalRequest</span></span> | <span data-ttu-id="89843-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-132">Boolean</span></span> | <span data-ttu-id="89843-133">指示传入的邮件是否必须为审批请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-133">Indicates whether an incoming message must be an approval request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-134">isAutomaticForward</span><span class="sxs-lookup"><span data-stu-id="89843-134">isAutomaticForward</span></span> | <span data-ttu-id="89843-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-135">Boolean</span></span> | <span data-ttu-id="89843-136">指示传入的邮件是否必须自动转发，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-136">Indicates whether an incoming message must be automatically forwarded in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-137">isAutomaticReply</span><span class="sxs-lookup"><span data-stu-id="89843-137">isAutomaticReply</span></span> | <span data-ttu-id="89843-138">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-138">Boolean</span></span> | <span data-ttu-id="89843-139">指示传入的邮件是否必须自动答复，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-139">Indicates whether an incoming message must be an auto reply in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-140">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="89843-140">isEncrypted</span></span> | <span data-ttu-id="89843-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-141">Boolean</span></span> | <span data-ttu-id="89843-142">指示传入的邮件是否必须加密，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-142">Indicates whether an incoming message must be encrypted in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-143">isMeetingRequest</span><span class="sxs-lookup"><span data-stu-id="89843-143">isMeetingRequest</span></span> | <span data-ttu-id="89843-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-144">Boolean</span></span> | <span data-ttu-id="89843-145">指示传入的邮件是否必须为会议请求，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-145">Indicates whether an incoming message must be a meeting request in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-146">isMeetingResponse</span><span class="sxs-lookup"><span data-stu-id="89843-146">isMeetingResponse</span></span> | <span data-ttu-id="89843-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-147">Boolean</span></span> | <span data-ttu-id="89843-148">指示传入的邮件是否必须为会议响应，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-148">Indicates whether an incoming message must be a meeting response in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-149">isNonDeliveryReport</span><span class="sxs-lookup"><span data-stu-id="89843-149">isNonDeliveryReport</span></span> | <span data-ttu-id="89843-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-150">Boolean</span></span> | <span data-ttu-id="89843-151">指示传入的邮件是否必须为未送达报告，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-151">Indicates whether an incoming message must be a non-delivery report in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-152">isPermissionControlled</span><span class="sxs-lookup"><span data-stu-id="89843-152">isPermissionControlled</span></span> | <span data-ttu-id="89843-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-153">Boolean</span></span> | <span data-ttu-id="89843-154">指示传入的邮件是否必须受权限控制（受 RMS 保护），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-154">Indicates whether an incoming message must be permission controlled (RMS-protected) in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-155">isReadReceipt</span><span class="sxs-lookup"><span data-stu-id="89843-155">isReadReceipt</span></span> | <span data-ttu-id="89843-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-156">Boolean</span></span> | <span data-ttu-id="89843-157">指示传入的邮件是否必须为已读回执，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-157">Indicates whether an incoming message must be a read receipt in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-158">isSigned</span><span class="sxs-lookup"><span data-stu-id="89843-158">isSigned</span></span> | <span data-ttu-id="89843-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-159">Boolean</span></span> | <span data-ttu-id="89843-160">指示传入的邮件是否必须有 S/MIME 签名，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-160">Indicates whether an incoming message must be S/MIME-signed in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-161">isVoicemail</span><span class="sxs-lookup"><span data-stu-id="89843-161">isVoicemail</span></span> | <span data-ttu-id="89843-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-162">Boolean</span></span> | <span data-ttu-id="89843-163">指示传入的邮件是否必须有语音邮件，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-163">Indicates whether an incoming message must be a voice mail in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-164">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="89843-164">messageActionFlag</span></span> | <span data-ttu-id="89843-165">messageActionFlag</span><span class="sxs-lookup"><span data-stu-id="89843-165">messageActionFlag</span></span>  | <span data-ttu-id="89843-166">表示出现在传入邮件上的 flag-for-action 值，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-166">Represents the flag-for-action value that appears on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="89843-167">可能的值为： `any`、 `call`、 `doNotForward` `followUp` `fyi` `forward` `noResponseNecessary` `read` `reply`、、、、、、、、 `review` `replyToAll`。</span><span class="sxs-lookup"><span data-stu-id="89843-167">The possible values are: `any`, `call`, `doNotForward`, `followUp`, `fyi`, `forward`, `noResponseNecessary`, `read`, `reply`, `replyToAll`, `review`.</span></span> |
| <span data-ttu-id="89843-168">notSentToMe</span><span class="sxs-lookup"><span data-stu-id="89843-168">notSentToMe</span></span> | <span data-ttu-id="89843-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-169">Boolean</span></span> | <span data-ttu-id="89843-170">指示邮箱所有者是否不能是传入邮件的收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-170">Indicates whether the owner of the mailbox must not be a recipient of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-171">recipientContains</span><span class="sxs-lookup"><span data-stu-id="89843-171">recipientContains</span></span> | <span data-ttu-id="89843-172">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-172">Collection(String)</span></span> | <span data-ttu-id="89843-173">表示出现在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-173">Represents the strings that appear in either the **toRecipients** or **ccRecipients** properties of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-174">senderContains</span><span class="sxs-lookup"><span data-stu-id="89843-174">senderContains</span></span> | <span data-ttu-id="89843-175">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-175">Collection(String)</span></span> | <span data-ttu-id="89843-176">表示出现在传入邮件的 **from** 属性中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-176">Represents the strings that appear in the **from** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-177">sensitivity</span><span class="sxs-lookup"><span data-stu-id="89843-177">sensitivity</span></span> | <span data-ttu-id="89843-178">敏感度</span><span class="sxs-lookup"><span data-stu-id="89843-178">sensitivity</span></span> | <span data-ttu-id="89843-179">表示必须在传入邮件上标记的敏感度级别，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-179">Represents the sensitivity level that must be stamped on an incoming message in order for the condition or exception to apply.</span></span> <span data-ttu-id="89843-180">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="89843-180">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span> |
| <span data-ttu-id="89843-181">sentCcMe</span><span class="sxs-lookup"><span data-stu-id="89843-181">sentCcMe</span></span> | <span data-ttu-id="89843-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-182">Boolean</span></span> | <span data-ttu-id="89843-183">指示邮箱所有者是否必须在传入邮件的 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-183">Indicates whether the owner of the mailbox must be in the **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-184">sentOnlyToMe</span><span class="sxs-lookup"><span data-stu-id="89843-184">sentOnlyToMe</span></span> | <span data-ttu-id="89843-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-185">Boolean</span></span> | <span data-ttu-id="89843-186">指示邮箱所有者是否必须是传入邮件的唯一收件人，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-186">Indicates whether the owner of the mailbox must be the only recipient in an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-187">sentToAddresses</span><span class="sxs-lookup"><span data-stu-id="89843-187">sentToAddresses</span></span> | <span data-ttu-id="89843-188">集合（[收件人](recipient.md)）</span><span class="sxs-lookup"><span data-stu-id="89843-188">Collection([recipient](recipient.md))</span></span> | <span data-ttu-id="89843-189">表示必须已向其发送传入邮件的电子邮件地址，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-189">Represents the email addresses that an incoming message must have been sent to in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-190">sentToMe</span><span class="sxs-lookup"><span data-stu-id="89843-190">sentToMe</span></span> | <span data-ttu-id="89843-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-191">Boolean</span></span> | <span data-ttu-id="89843-192">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-192">Indicates whether the owner of the mailbox must be in the **toRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-193">sentToOrCcMe</span><span class="sxs-lookup"><span data-stu-id="89843-193">sentToOrCcMe</span></span> | <span data-ttu-id="89843-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="89843-194">Boolean</span></span> | <span data-ttu-id="89843-195">指示邮箱所有者是否必须在传入邮件的 **toRecipients** 或 **ccRecipients** 属性中，以便条件或异常情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-195">Indicates whether the owner of the mailbox must be in either a **toRecipients** or **ccRecipients** property of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-196">subjectContains</span><span class="sxs-lookup"><span data-stu-id="89843-196">subjectContains</span></span> | <span data-ttu-id="89843-197">集合（字符串）</span><span class="sxs-lookup"><span data-stu-id="89843-197">Collection(String)</span></span> | <span data-ttu-id="89843-198">表示出现在传入邮件主题中的字符串，以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-198">Represents the strings that appear in the subject of an incoming message in order for the condition or exception to apply.</span></span> |
| <span data-ttu-id="89843-199">withinSizeRange</span><span class="sxs-lookup"><span data-stu-id="89843-199">withinSizeRange</span></span> | [<span data-ttu-id="89843-200">sizeRange</span><span class="sxs-lookup"><span data-stu-id="89843-200">sizeRange</span></span>](sizerange.md) | <span data-ttu-id="89843-201">表示传入邮件必须介于其中的最小大小和最大大小（以千字节为单位），以便条件或例外情况适用。</span><span class="sxs-lookup"><span data-stu-id="89843-201">Represents the minimum and maximum sizes (in kilobytes) that an incoming message must fall in between in order for the condition or exception to apply.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="89843-202">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89843-202">JSON representation</span></span>
<span data-ttu-id="89843-203">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89843-203">Here is a JSON representation of the resource.</span></span>

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
