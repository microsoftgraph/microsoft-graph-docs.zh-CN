---
title: eventMessageRequest 资源类型
description: 表示会议请求的邮件。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: ead65f036fe5537b7e349124b2771eff575be22f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333942"
---
# <a name="eventmessagerequest-resource-type"></a><span data-ttu-id="2ecdf-103">eventMessageRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ecdf-103">eventMessageRequest resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ecdf-104">表示会议请求的邮件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-104">A message that represents a meeting request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ecdf-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ecdf-105">JSON representation</span></span>

<span data-ttu-id="2ecdf-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [
    "attachments",
    "event",
    "extensions",
    "previousLocation",
    "previousStartDateTime",
    "previousEndDateTime"
  ],
  "@odata.type": "microsoft.graph.eventMessageRequest"
}-->

```json
{
  "bccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "ccRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "changeKey": "string",
  "conversationId": "string",
  "createdDateTime": "String (timestamp)",
  "endDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "from": {"@odata.type": "microsoft.graph.recipient"},
  "hasAttachments": true,
  "id": "string (identifier)",
  "importance": "String",
  "inferenceClassification": "String",
  "isDeliveryReceiptRequested": true,
  "isDraft": true,
  "isOutOfDate": "Boolean",
  "isRead": true,
  "isReadReceiptRequested": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "meetingMessageType": "microsoft.graph.meetingMessageType",
  "parentFolderId": "string",
  "previousEndDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "previousLocation": {"@odata.type": "microsoft.graph.location"},
  "previousStartDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "receivedDateTime": "String (timestamp)",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "replyTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "sender": {"@odata.type": "microsoft.graph.recipient"},
  "sentDateTime": "String (timestamp)",
  "startDateTime": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "toRecipients": [{"@odata.type": "microsoft.graph.recipient"}],
  "type": "string",
  "uniqueBody": {"@odata.type": "microsoft.graph.itemBody"},
  "webLink": "string"
}

```
## <a name="properties"></a><span data-ttu-id="2ecdf-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ecdf-107">Properties</span></span>
| <span data-ttu-id="2ecdf-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ecdf-108">Property</span></span>     | <span data-ttu-id="2ecdf-109">类型</span><span class="sxs-lookup"><span data-stu-id="2ecdf-109">Type</span></span>   |<span data-ttu-id="2ecdf-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ecdf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ecdf-111">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="2ecdf-111">bccRecipients</span></span>|<span data-ttu-id="2ecdf-112">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2ecdf-112">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="2ecdf-113">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-113">The Bcc: recipients for the message.</span></span>|
|<span data-ttu-id="2ecdf-114">body</span><span class="sxs-lookup"><span data-stu-id="2ecdf-114">body</span></span>|[<span data-ttu-id="2ecdf-115">itemBody</span><span class="sxs-lookup"><span data-stu-id="2ecdf-115">itemBody</span></span>](itembody.md)|<span data-ttu-id="2ecdf-116">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-116">The body of the message.</span></span>|
|<span data-ttu-id="2ecdf-117">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="2ecdf-117">bodyPreview</span></span>|<span data-ttu-id="2ecdf-118">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-118">String</span></span>|<span data-ttu-id="2ecdf-119">邮件正文中的前 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-119">The first 255 characters of the message body.</span></span>|
|<span data-ttu-id="2ecdf-120">类别</span><span class="sxs-lookup"><span data-stu-id="2ecdf-120">categories</span></span>|<span data-ttu-id="2ecdf-121">String collection</span><span class="sxs-lookup"><span data-stu-id="2ecdf-121">String collection</span></span>|<span data-ttu-id="2ecdf-122">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-122">The categories associated with the message.</span></span>|
|<span data-ttu-id="2ecdf-123">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="2ecdf-123">ccRecipients</span></span>|<span data-ttu-id="2ecdf-124">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2ecdf-124">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="2ecdf-125">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-125">The Cc: recipients for the message.</span></span>|
|<span data-ttu-id="2ecdf-126">changeKey</span><span class="sxs-lookup"><span data-stu-id="2ecdf-126">changeKey</span></span>|<span data-ttu-id="2ecdf-127">字符串</span><span class="sxs-lookup"><span data-stu-id="2ecdf-127">String</span></span>|<span data-ttu-id="2ecdf-128">邮件的版本。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-128">The version of the message.</span></span>|
|<span data-ttu-id="2ecdf-129">conversationId</span><span class="sxs-lookup"><span data-stu-id="2ecdf-129">conversationId</span></span>|<span data-ttu-id="2ecdf-130">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-130">String</span></span>|<span data-ttu-id="2ecdf-131">电子邮件所属的对话的 ID。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-131">The ID of the conversation the email belongs to.</span></span>|
|<span data-ttu-id="2ecdf-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-132">createdDateTime</span></span>|<span data-ttu-id="2ecdf-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ecdf-133">DateTimeOffset</span></span>|<span data-ttu-id="2ecdf-134">创建邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-134">The date and time the message was created.</span></span>|
|<span data-ttu-id="2ecdf-135">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-135">endDateTime</span></span>|[<span data-ttu-id="2ecdf-136">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ecdf-136">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ecdf-137">请求的会议的结束时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-137">The end time of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-138">发件人</span><span class="sxs-lookup"><span data-stu-id="2ecdf-138">from</span></span>|[<span data-ttu-id="2ecdf-139">recipient</span><span class="sxs-lookup"><span data-stu-id="2ecdf-139">recipient</span></span>](recipient.md)|<span data-ttu-id="2ecdf-140">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-140">The mailbox owner and sender of the message.</span></span>|
|<span data-ttu-id="2ecdf-141">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="2ecdf-141">hasAttachments</span></span>|<span data-ttu-id="2ecdf-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-142">Boolean</span></span>|<span data-ttu-id="2ecdf-143">指示邮件是否包含附件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-143">Indicates whether the message has attachments.</span></span>|
|<span data-ttu-id="2ecdf-144">id</span><span class="sxs-lookup"><span data-stu-id="2ecdf-144">id</span></span>|<span data-ttu-id="2ecdf-145">字串符号</span><span class="sxs-lookup"><span data-stu-id="2ecdf-145">String</span></span>|<span data-ttu-id="2ecdf-146">只读。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-146">Read-only.</span></span>|
|<span data-ttu-id="2ecdf-147">importance</span><span class="sxs-lookup"><span data-stu-id="2ecdf-147">importance</span></span>|<span data-ttu-id="2ecdf-148">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-148">String</span></span>| <span data-ttu-id="2ecdf-149">邮件的重要性：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-149">The importance of the message: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="2ecdf-150">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="2ecdf-150">inferenceClassification</span></span>|<span data-ttu-id="2ecdf-151">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-151">String</span></span>| <span data-ttu-id="2ecdf-152">可取值为：`Focused`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-152">Possible values are: `Focused`, `Other`.</span></span>|
|<span data-ttu-id="2ecdf-153">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2ecdf-153">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="2ecdf-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-154">Boolean</span></span>|<span data-ttu-id="2ecdf-155">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-155">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2ecdf-156">isDraft</span><span class="sxs-lookup"><span data-stu-id="2ecdf-156">isDraft</span></span>|<span data-ttu-id="2ecdf-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-157">Boolean</span></span>|<span data-ttu-id="2ecdf-p101">指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p101">Indicates whether the message is a draft. A message is a draft if it hasn't been sent yet.</span></span>|
|<span data-ttu-id="2ecdf-160">isOutOfDate</span><span class="sxs-lookup"><span data-stu-id="2ecdf-160">isOutOfDate</span></span>|<span data-ttu-id="2ecdf-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-161">Boolean</span></span>|<span data-ttu-id="2ecdf-162">指示此会议请求是否已由较新的请求发出。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-162">Indicates whether this meeting request has been made out-of-date by a more recent request.</span></span>|
|<span data-ttu-id="2ecdf-163">isRead</span><span class="sxs-lookup"><span data-stu-id="2ecdf-163">isRead</span></span>|<span data-ttu-id="2ecdf-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-164">Boolean</span></span>|<span data-ttu-id="2ecdf-165">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-165">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="2ecdf-166">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="2ecdf-166">isReadReceiptRequested</span></span>|<span data-ttu-id="2ecdf-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ecdf-167">Boolean</span></span>|<span data-ttu-id="2ecdf-168">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-168">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="2ecdf-169">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-169">lastModifiedDateTime</span></span>|<span data-ttu-id="2ecdf-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ecdf-170">DateTimeOffset</span></span>|<span data-ttu-id="2ecdf-171">上次更改邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-171">The date and time the message was last changed.</span></span>|
|<span data-ttu-id="2ecdf-172">位置</span><span class="sxs-lookup"><span data-stu-id="2ecdf-172">location</span></span>|[<span data-ttu-id="2ecdf-173">位置</span><span class="sxs-lookup"><span data-stu-id="2ecdf-173">Location</span></span>](location.md)|<span data-ttu-id="2ecdf-174">请求的会议的位置。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-174">The location of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-175">meetingMessageType</span><span class="sxs-lookup"><span data-stu-id="2ecdf-175">meetingMessageType</span></span>|<span data-ttu-id="2ecdf-176">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-176">String</span></span>| <span data-ttu-id="2ecdf-177">事件消息的类型：`none`、`meetingRequest`、`meetingCancelled`、`meetingAccepted`、`meetingTentativelyAccepted`、`meetingDeclined`。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-177">The type of event message: `none`, `meetingRequest`, `meetingCancelled`, `meetingAccepted`, `meetingTentativelyAccepted`, `meetingDeclined`.</span></span>|
|<span data-ttu-id="2ecdf-178">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="2ecdf-178">parentFolderId</span></span>|<span data-ttu-id="2ecdf-179">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-179">String</span></span>|<span data-ttu-id="2ecdf-180">邮件的父 MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-180">The unique identifier for the message's parent mailFolder.</span></span>|
|<span data-ttu-id="2ecdf-181">previousEndDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-181">previousEndDateTime</span></span>|[<span data-ttu-id="2ecdf-182">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ecdf-182">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ecdf-183">请求的会议的上一次结束时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-183">The previous end time of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-184">previousLocation</span><span class="sxs-lookup"><span data-stu-id="2ecdf-184">previousLocation</span></span>|[<span data-ttu-id="2ecdf-185">位置</span><span class="sxs-lookup"><span data-stu-id="2ecdf-185">Location</span></span>](location.md)|<span data-ttu-id="2ecdf-186">所请求会议的上一个位置。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-186">The previous location of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-187">previousStartDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-187">previousStartDateTime</span></span>|[<span data-ttu-id="2ecdf-188">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ecdf-188">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ecdf-189">请求的会议的上一次开始时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-189">The previous start time of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-190">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-190">receivedDateTime</span></span>|<span data-ttu-id="2ecdf-191">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ecdf-191">DateTimeOffset</span></span>|<span data-ttu-id="2ecdf-192">收到邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-192">The date and time the message was received.</span></span>|
|<span data-ttu-id="2ecdf-193">recurrence</span><span class="sxs-lookup"><span data-stu-id="2ecdf-193">recurrence</span></span>|[<span data-ttu-id="2ecdf-194">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="2ecdf-194">PatternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="2ecdf-195">请求的会议的定期模式。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-195">The recurrence pattern of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-196">replyTo</span><span class="sxs-lookup"><span data-stu-id="2ecdf-196">replyTo</span></span>|<span data-ttu-id="2ecdf-197">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2ecdf-197">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="2ecdf-198">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-198">The email addresses to use when replying.</span></span>|
|<span data-ttu-id="2ecdf-199">sender</span><span class="sxs-lookup"><span data-stu-id="2ecdf-199">sender</span></span>|[<span data-ttu-id="2ecdf-200">recipient</span><span class="sxs-lookup"><span data-stu-id="2ecdf-200">recipient</span></span>](recipient.md)|<span data-ttu-id="2ecdf-201">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-201">The account that is actually used to generate the message.</span></span>|
|<span data-ttu-id="2ecdf-202">sentDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-202">sentDateTime</span></span>|<span data-ttu-id="2ecdf-203">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ecdf-203">DateTimeOffset</span></span>|<span data-ttu-id="2ecdf-204">发送邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-204">The date and time the message was sent.</span></span>|
|<span data-ttu-id="2ecdf-205">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2ecdf-205">startDateTime</span></span>|[<span data-ttu-id="2ecdf-206">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="2ecdf-206">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="2ecdf-207">请求的会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-207">The start time of the requested meeting.</span></span>|
|<span data-ttu-id="2ecdf-208">subject</span><span class="sxs-lookup"><span data-stu-id="2ecdf-208">subject</span></span>|<span data-ttu-id="2ecdf-209">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-209">String</span></span>|<span data-ttu-id="2ecdf-210">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-210">The subject of the message.</span></span>|
|<span data-ttu-id="2ecdf-211">toRecipients</span><span class="sxs-lookup"><span data-stu-id="2ecdf-211">toRecipients</span></span>|<span data-ttu-id="2ecdf-212">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="2ecdf-212">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="2ecdf-213">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-213">The To: recipients for the message.</span></span>|
|<span data-ttu-id="2ecdf-214">type</span><span class="sxs-lookup"><span data-stu-id="2ecdf-214">type</span></span>|<span data-ttu-id="2ecdf-215">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-215">String</span></span>|<span data-ttu-id="2ecdf-216">所需会议的类型: `singleInstance`、 `occurence`、 `exception`、 `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-216">The type of requested meeting: `singleInstance`, `occurence`, `exception`, `seriesMaster`.</span></span>|
|<span data-ttu-id="2ecdf-217">uniqueBody</span><span class="sxs-lookup"><span data-stu-id="2ecdf-217">uniqueBody</span></span>|[<span data-ttu-id="2ecdf-218">itemBody</span><span class="sxs-lookup"><span data-stu-id="2ecdf-218">itemBody</span></span>](itembody.md)|<span data-ttu-id="2ecdf-219">当前邮件专用的邮件正文部分。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-219">The part of the body of the message that is unique to the current message.</span></span>|
|<span data-ttu-id="2ecdf-220">webLink</span><span class="sxs-lookup"><span data-stu-id="2ecdf-220">webLink</span></span>|<span data-ttu-id="2ecdf-221">String</span><span class="sxs-lookup"><span data-stu-id="2ecdf-221">String</span></span>|<span data-ttu-id="2ecdf-222">要在 Outlook Web App 中打开邮件的 URL。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-222">The URL to open the message in Outlook Web App.</span></span><br><br><span data-ttu-id="2ecdf-p102">可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p102">You can append an ispopout argument to the end of the URL to change how the message is displayed. If ispopout is not present or if it is set to 1, then the message is shown in a popout window. If ispopout is set to 0, then the browser will show the message in the Outlook Web App review pane.</span></span><br><br><span data-ttu-id="2ecdf-p103">如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p103">The message will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br><br><span data-ttu-id="2ecdf-228">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-228">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ecdf-229">关系</span><span class="sxs-lookup"><span data-stu-id="2ecdf-229">Relationships</span></span>
| <span data-ttu-id="2ecdf-230">关系</span><span class="sxs-lookup"><span data-stu-id="2ecdf-230">Relationship</span></span> | <span data-ttu-id="2ecdf-231">类型</span><span class="sxs-lookup"><span data-stu-id="2ecdf-231">Type</span></span>   |<span data-ttu-id="2ecdf-232">说明</span><span class="sxs-lookup"><span data-stu-id="2ecdf-232">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2ecdf-233">attachments</span><span class="sxs-lookup"><span data-stu-id="2ecdf-233">attachments</span></span>|<span data-ttu-id="2ecdf-234">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ecdf-234">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="2ecdf-p104">只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p104">Read-only. Nullable.</span></span>|
|<span data-ttu-id="2ecdf-237">event</span><span class="sxs-lookup"><span data-stu-id="2ecdf-237">event</span></span>|[<span data-ttu-id="2ecdf-238">事件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-238">Event</span></span>](event.md)| <span data-ttu-id="2ecdf-p105">与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p105">The event associated with the event message. The assumption for attendees or room resources is that the Calendar Attendant is set to automatically update the calendar with an event when meeting request event messages arrive. Navigation property.  Read-only.</span></span>|
|<span data-ttu-id="2ecdf-243">extensions</span><span class="sxs-lookup"><span data-stu-id="2ecdf-243">extensions</span></span>|<span data-ttu-id="2ecdf-244">[Extension](extension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ecdf-244">[Extension](extension.md) collection</span></span>| <span data-ttu-id="2ecdf-245">只读。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-245">Read-only.</span></span> <span data-ttu-id="2ecdf-246">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-246">Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="2ecdf-247">方法</span><span class="sxs-lookup"><span data-stu-id="2ecdf-247">Methods</span></span>

| <span data-ttu-id="2ecdf-248">方法</span><span class="sxs-lookup"><span data-stu-id="2ecdf-248">Method</span></span>           | <span data-ttu-id="2ecdf-249">返回类型</span><span class="sxs-lookup"><span data-stu-id="2ecdf-249">Return Type</span></span>    |<span data-ttu-id="2ecdf-250">说明</span><span class="sxs-lookup"><span data-stu-id="2ecdf-250">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2ecdf-251">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="2ecdf-251">Get eventMessage</span></span>](../api/eventmessage-get.md) | [<span data-ttu-id="2ecdf-252">eventMessage</span><span class="sxs-lookup"><span data-stu-id="2ecdf-252">eventMessage</span></span>](eventmessage.md) |<span data-ttu-id="2ecdf-253">读取 eventmessage 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-253">Read properties and relationships of eventMessage object.</span></span>|
|[<span data-ttu-id="2ecdf-254">创建附件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-254">Create Attachment</span></span>](../api/eventmessage-post-attachments.md) |[<span data-ttu-id="2ecdf-255">附件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-255">Attachment</span></span>](attachment.md)| <span data-ttu-id="2ecdf-256">通过发布到附件集合创建新附件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-256">Create a new Attachment by posting to the attachments collection.</span></span>|
|[<span data-ttu-id="2ecdf-257">列出附件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-257">List attachments</span></span>](../api/eventmessage-list-attachments.md) |<span data-ttu-id="2ecdf-258">[Attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2ecdf-258">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="2ecdf-259">获取附件对象集合。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-259">Get a Attachment object collection.</span></span>|
|[<span data-ttu-id="2ecdf-260">更新</span><span class="sxs-lookup"><span data-stu-id="2ecdf-260">Update</span></span>](../api/eventmessage-update.md) | [<span data-ttu-id="2ecdf-261">eventMessage</span><span class="sxs-lookup"><span data-stu-id="2ecdf-261">eventMessage</span></span>](eventmessage.md)  |<span data-ttu-id="2ecdf-262">更新 eventMessage 对象。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-262">Update eventMessage object.</span></span> |
|[<span data-ttu-id="2ecdf-263">删除</span><span class="sxs-lookup"><span data-stu-id="2ecdf-263">Delete</span></span>](../api/eventmessage-delete.md) | <span data-ttu-id="2ecdf-264">None</span><span class="sxs-lookup"><span data-stu-id="2ecdf-264">None</span></span> |<span data-ttu-id="2ecdf-265">更新 eventMessage 对象。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-265">Delete eventMessage object.</span></span> |
|[<span data-ttu-id="2ecdf-266">复制</span><span class="sxs-lookup"><span data-stu-id="2ecdf-266">copy</span></span>](../api/message-copy.md)|[<span data-ttu-id="2ecdf-267">邮件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-267">Message</span></span>](message.md)||
|[<span data-ttu-id="2ecdf-268">createForward</span><span class="sxs-lookup"><span data-stu-id="2ecdf-268">createForward</span></span>](../api/message-createforward.md)|[<span data-ttu-id="2ecdf-269">邮件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-269">Message</span></span>](message.md)||
|[<span data-ttu-id="2ecdf-270">createReply</span><span class="sxs-lookup"><span data-stu-id="2ecdf-270">createReply</span></span>](../api/message-createreply.md)|[<span data-ttu-id="2ecdf-271">邮件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-271">Message</span></span>](message.md)||
|[<span data-ttu-id="2ecdf-272">createReplyAll</span><span class="sxs-lookup"><span data-stu-id="2ecdf-272">createReplyAll</span></span>](../api/message-createreplyall.md)|[<span data-ttu-id="2ecdf-273">Message</span><span class="sxs-lookup"><span data-stu-id="2ecdf-273">Message</span></span>](message.md)||
|[<span data-ttu-id="2ecdf-274">转发</span><span class="sxs-lookup"><span data-stu-id="2ecdf-274">forward</span></span>](../api/message-forward.md)|<span data-ttu-id="2ecdf-275">无</span><span class="sxs-lookup"><span data-stu-id="2ecdf-275">None</span></span>|<span data-ttu-id="2ecdf-276">转发邮件。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-276">Forwards a message.</span></span> <span data-ttu-id="2ecdf-277">然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-277">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="2ecdf-278">移动</span><span class="sxs-lookup"><span data-stu-id="2ecdf-278">move</span></span>](../api/message-move.md)|[<span data-ttu-id="2ecdf-279">邮件</span><span class="sxs-lookup"><span data-stu-id="2ecdf-279">Message</span></span>](message.md)|<span data-ttu-id="2ecdf-280">将邮件移动到 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-280">Move the message to a mailFolder.</span></span>|
|[<span data-ttu-id="2ecdf-281">回复</span><span class="sxs-lookup"><span data-stu-id="2ecdf-281">reply</span></span>](../api/message-reply.md)|<span data-ttu-id="2ecdf-282">无</span><span class="sxs-lookup"><span data-stu-id="2ecdf-282">None</span></span>|<span data-ttu-id="2ecdf-283">Replys 到邮件的发件人。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-283">Replys to the sender of a message.</span></span> <span data-ttu-id="2ecdf-284">然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-284">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="2ecdf-285">全部回复</span><span class="sxs-lookup"><span data-stu-id="2ecdf-285">replyAll</span></span>](../api/message-replyall.md)|<span data-ttu-id="2ecdf-286">无</span><span class="sxs-lookup"><span data-stu-id="2ecdf-286">None</span></span>|<span data-ttu-id="2ecdf-p109">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p109">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="2ecdf-289">发送</span><span class="sxs-lookup"><span data-stu-id="2ecdf-289">send</span></span>](../api/message-send.md)|<span data-ttu-id="2ecdf-290">无</span><span class="sxs-lookup"><span data-stu-id="2ecdf-290">None</span></span>|<span data-ttu-id="2ecdf-p110">发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2ecdf-p110">Sends a previously created message draft. The message is then saved in the Sent Items folder.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
