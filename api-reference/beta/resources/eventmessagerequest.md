---
title: eventMessageRequest 资源类型
description: 代表一个会议请求消息。
author: angelgolfer-ms
localization_priority: Normal
ms.openlocfilehash: 6a4af3bef767213c977dde1195c89d1de02a0cf8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844021"
---
# <a name="eventmessagerequest-resource-type"></a><span data-ttu-id="22d9b-103">eventMessageRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="22d9b-103">eventMessageRequest resource type</span></span>

> <span data-ttu-id="22d9b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="22d9b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22d9b-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="22d9b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="22d9b-106">代表一个会议请求消息。</span><span class="sxs-lookup"><span data-stu-id="22d9b-106">A message that represents a meeting request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22d9b-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22d9b-107">JSON representation</span></span>

<span data-ttu-id="22d9b-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22d9b-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
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
## <a name="properties"></a><span data-ttu-id="22d9b-109">属性</span><span class="sxs-lookup"><span data-stu-id="22d9b-109">Properties</span></span>
| <span data-ttu-id="22d9b-110">属性</span><span class="sxs-lookup"><span data-stu-id="22d9b-110">Property</span></span>     | <span data-ttu-id="22d9b-111">类型</span><span class="sxs-lookup"><span data-stu-id="22d9b-111">Type</span></span>   |<span data-ttu-id="22d9b-112">说明</span><span class="sxs-lookup"><span data-stu-id="22d9b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d9b-113">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="22d9b-113">bccRecipients</span></span>|<span data-ttu-id="22d9b-114">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="22d9b-114">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="22d9b-115">邮件的密件抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="22d9b-115">The Bcc: recipients for the message.</span></span>|
|<span data-ttu-id="22d9b-116">body</span><span class="sxs-lookup"><span data-stu-id="22d9b-116">body</span></span>|[<span data-ttu-id="22d9b-117">itemBody</span><span class="sxs-lookup"><span data-stu-id="22d9b-117">itemBody</span></span>](itembody.md)|<span data-ttu-id="22d9b-118">邮件的正文。</span><span class="sxs-lookup"><span data-stu-id="22d9b-118">The body of the message.</span></span>|
|<span data-ttu-id="22d9b-119">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="22d9b-119">bodyPreview</span></span>|<span data-ttu-id="22d9b-120">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-120">String</span></span>|<span data-ttu-id="22d9b-121">邮件正文中的前 255 个字符。</span><span class="sxs-lookup"><span data-stu-id="22d9b-121">The first 255 characters of the message body.</span></span>|
|<span data-ttu-id="22d9b-122">categories</span><span class="sxs-lookup"><span data-stu-id="22d9b-122">categories</span></span>|<span data-ttu-id="22d9b-123">String collection</span><span class="sxs-lookup"><span data-stu-id="22d9b-123">String collection</span></span>|<span data-ttu-id="22d9b-124">与邮件关联的类别。</span><span class="sxs-lookup"><span data-stu-id="22d9b-124">The categories associated with the message.</span></span>|
|<span data-ttu-id="22d9b-125">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="22d9b-125">ccRecipients</span></span>|<span data-ttu-id="22d9b-126">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="22d9b-126">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="22d9b-127">邮件的抄送收件人。</span><span class="sxs-lookup"><span data-stu-id="22d9b-127">The Cc: recipients for the message.</span></span>|
|<span data-ttu-id="22d9b-128">changeKey</span><span class="sxs-lookup"><span data-stu-id="22d9b-128">changeKey</span></span>|<span data-ttu-id="22d9b-129">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-129">String</span></span>|<span data-ttu-id="22d9b-130">邮件的版本。</span><span class="sxs-lookup"><span data-stu-id="22d9b-130">The version of the message.</span></span>|
|<span data-ttu-id="22d9b-131">conversationId</span><span class="sxs-lookup"><span data-stu-id="22d9b-131">conversationId</span></span>|<span data-ttu-id="22d9b-132">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-132">String</span></span>|<span data-ttu-id="22d9b-133">电子邮件所属的对话的 ID。</span><span class="sxs-lookup"><span data-stu-id="22d9b-133">The ID of the conversation the email belongs to.</span></span>|
|<span data-ttu-id="22d9b-134">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-134">createdDateTime</span></span>|<span data-ttu-id="22d9b-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d9b-135">DateTimeOffset</span></span>|<span data-ttu-id="22d9b-136">创建邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-136">The date and time the message was created.</span></span>|
|<span data-ttu-id="22d9b-137">endDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-137">endDateTime</span></span>|[<span data-ttu-id="22d9b-138">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="22d9b-138">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="22d9b-139">请求会议结束时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-139">The end time of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-140">发件人</span><span class="sxs-lookup"><span data-stu-id="22d9b-140">from</span></span>|[<span data-ttu-id="22d9b-141">recipient</span><span class="sxs-lookup"><span data-stu-id="22d9b-141">recipient</span></span>](recipient.md)|<span data-ttu-id="22d9b-142">邮箱所有者和邮件发件人。</span><span class="sxs-lookup"><span data-stu-id="22d9b-142">The mailbox owner and sender of the message.</span></span>|
|<span data-ttu-id="22d9b-143">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="22d9b-143">hasAttachments</span></span>|<span data-ttu-id="22d9b-144">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-144">Boolean</span></span>|<span data-ttu-id="22d9b-145">指示邮件是否包含附件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-145">Indicates whether the message has attachments.</span></span>|
|<span data-ttu-id="22d9b-146">id</span><span class="sxs-lookup"><span data-stu-id="22d9b-146">id</span></span>|<span data-ttu-id="22d9b-147">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-147">String</span></span>|<span data-ttu-id="22d9b-148">只读。</span><span class="sxs-lookup"><span data-stu-id="22d9b-148">Read-only.</span></span>|
|<span data-ttu-id="22d9b-149">importance</span><span class="sxs-lookup"><span data-stu-id="22d9b-149">importance</span></span>|<span data-ttu-id="22d9b-150">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-150">String</span></span>| <span data-ttu-id="22d9b-151">邮件的重要性：`Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="22d9b-151">The importance of the message: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="22d9b-152">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="22d9b-152">inferenceClassification</span></span>|<span data-ttu-id="22d9b-153">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-153">String</span></span>| <span data-ttu-id="22d9b-154">可取值为：`Focused`、`Other`。</span><span class="sxs-lookup"><span data-stu-id="22d9b-154">Possible values are: `Focused`, `Other`.</span></span>|
|<span data-ttu-id="22d9b-155">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="22d9b-155">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="22d9b-156">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-156">Boolean</span></span>|<span data-ttu-id="22d9b-157">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="22d9b-157">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="22d9b-158">isDraft</span><span class="sxs-lookup"><span data-stu-id="22d9b-158">isDraft</span></span>|<span data-ttu-id="22d9b-159">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-159">Boolean</span></span>|<span data-ttu-id="22d9b-p102">指示邮件是否为草稿。如果尚未发送，则此邮件是一封草稿。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p102">Indicates whether the message is a draft. A message is a draft if it hasn't been sent yet.</span></span>|
|<span data-ttu-id="22d9b-162">isOutOfDate</span><span class="sxs-lookup"><span data-stu-id="22d9b-162">isOutOfDate</span></span>|<span data-ttu-id="22d9b-163">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-163">Boolean</span></span>|<span data-ttu-id="22d9b-164">指示是否此会议请求已过期较新的请求。</span><span class="sxs-lookup"><span data-stu-id="22d9b-164">Indicates whether this meeting request has been made out-of-date by a more recent request.</span></span>|
|<span data-ttu-id="22d9b-165">isRead</span><span class="sxs-lookup"><span data-stu-id="22d9b-165">isRead</span></span>|<span data-ttu-id="22d9b-166">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-166">Boolean</span></span>|<span data-ttu-id="22d9b-167">指示是否已阅读该邮件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-167">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="22d9b-168">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="22d9b-168">isReadReceiptRequested</span></span>|<span data-ttu-id="22d9b-169">布尔</span><span class="sxs-lookup"><span data-stu-id="22d9b-169">Boolean</span></span>|<span data-ttu-id="22d9b-170">指示是否需要发送邮件已读回执。</span><span class="sxs-lookup"><span data-stu-id="22d9b-170">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="22d9b-171">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-171">lastModifiedDateTime</span></span>|<span data-ttu-id="22d9b-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d9b-172">DateTimeOffset</span></span>|<span data-ttu-id="22d9b-173">上次更改邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-173">The date and time the message was last changed.</span></span>|
|<span data-ttu-id="22d9b-174">位置</span><span class="sxs-lookup"><span data-stu-id="22d9b-174">location</span></span>|[<span data-ttu-id="22d9b-175">位置</span><span class="sxs-lookup"><span data-stu-id="22d9b-175">Location</span></span>](location.md)|<span data-ttu-id="22d9b-176">请求会议的位置。</span><span class="sxs-lookup"><span data-stu-id="22d9b-176">The location of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-177">meetingMessageType</span><span class="sxs-lookup"><span data-stu-id="22d9b-177">meetingMessageType</span></span>|<span data-ttu-id="22d9b-178">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-178">String</span></span>| <span data-ttu-id="22d9b-179">事件消息的类型：`None`、`MeetingRequest`、`MeetingCancelled`、`MeetingAccepted`、`MeetingTenativelyAccepted`、`MeetingDeclined`。</span><span class="sxs-lookup"><span data-stu-id="22d9b-179">The type of event message: `None`, `MeetingRequest`, `MeetingCancelled`, `MeetingAccepted`, `MeetingTenativelyAccepted`, `MeetingDeclined`.</span></span>|
|<span data-ttu-id="22d9b-180">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="22d9b-180">parentFolderId</span></span>|<span data-ttu-id="22d9b-181">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-181">String</span></span>|<span data-ttu-id="22d9b-182">邮件的父 MailFolder 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="22d9b-182">The unique identifier for the message's parent mailFolder.</span></span>|
|<span data-ttu-id="22d9b-183">previousEndDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-183">previousEndDateTime</span></span>|[<span data-ttu-id="22d9b-184">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="22d9b-184">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="22d9b-185">以前的请求的会议的结束时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-185">The previous end time of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-186">previousLocation</span><span class="sxs-lookup"><span data-stu-id="22d9b-186">previousLocation</span></span>|[<span data-ttu-id="22d9b-187">Location</span><span class="sxs-lookup"><span data-stu-id="22d9b-187">Location</span></span>](location.md)|<span data-ttu-id="22d9b-188">请求会议的上一位置。</span><span class="sxs-lookup"><span data-stu-id="22d9b-188">The previous location of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-189">previousStartDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-189">previousStartDateTime</span></span>|[<span data-ttu-id="22d9b-190">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="22d9b-190">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="22d9b-191">以前的请求的会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-191">The previous start time of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-192">receivedDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-192">receivedDateTime</span></span>|<span data-ttu-id="22d9b-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d9b-193">DateTimeOffset</span></span>|<span data-ttu-id="22d9b-194">收到邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-194">The date and time the message was received.</span></span>|
|<span data-ttu-id="22d9b-195">recurrence</span><span class="sxs-lookup"><span data-stu-id="22d9b-195">recurrence</span></span>|[<span data-ttu-id="22d9b-196">PatternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="22d9b-196">PatternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="22d9b-197">请求会议定期模式。</span><span class="sxs-lookup"><span data-stu-id="22d9b-197">The recurrence pattern of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-198">replyTo</span><span class="sxs-lookup"><span data-stu-id="22d9b-198">replyTo</span></span>|<span data-ttu-id="22d9b-199">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="22d9b-199">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="22d9b-200">在答复时使用的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="22d9b-200">The email addresses to use when replying.</span></span>|
|<span data-ttu-id="22d9b-201">sender</span><span class="sxs-lookup"><span data-stu-id="22d9b-201">sender</span></span>|[<span data-ttu-id="22d9b-202">recipient</span><span class="sxs-lookup"><span data-stu-id="22d9b-202">recipient</span></span>](recipient.md)|<span data-ttu-id="22d9b-203">实际用于生成邮件的帐户。</span><span class="sxs-lookup"><span data-stu-id="22d9b-203">The account that is actually used to generate the message.</span></span>|
|<span data-ttu-id="22d9b-204">sentDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-204">sentDateTime</span></span>|<span data-ttu-id="22d9b-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22d9b-205">DateTimeOffset</span></span>|<span data-ttu-id="22d9b-206">发送邮件的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-206">The date and time the message was sent.</span></span>|
|<span data-ttu-id="22d9b-207">startDateTime</span><span class="sxs-lookup"><span data-stu-id="22d9b-207">startDateTime</span></span>|[<span data-ttu-id="22d9b-208">DateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="22d9b-208">DateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="22d9b-209">请求的会议的开始时间。</span><span class="sxs-lookup"><span data-stu-id="22d9b-209">The start time of the requested meeting.</span></span>|
|<span data-ttu-id="22d9b-210">subject</span><span class="sxs-lookup"><span data-stu-id="22d9b-210">subject</span></span>|<span data-ttu-id="22d9b-211">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-211">String</span></span>|<span data-ttu-id="22d9b-212">邮件的主题。</span><span class="sxs-lookup"><span data-stu-id="22d9b-212">The subject of the message.</span></span>|
|<span data-ttu-id="22d9b-213">toRecipients</span><span class="sxs-lookup"><span data-stu-id="22d9b-213">toRecipients</span></span>|<span data-ttu-id="22d9b-214">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="22d9b-214">[recipient](recipient.md) collection</span></span>|<span data-ttu-id="22d9b-215">邮件的收件人。</span><span class="sxs-lookup"><span data-stu-id="22d9b-215">The To: recipients for the message.</span></span>|
|<span data-ttu-id="22d9b-216">type</span><span class="sxs-lookup"><span data-stu-id="22d9b-216">type</span></span>|<span data-ttu-id="22d9b-217">字符串</span><span class="sxs-lookup"><span data-stu-id="22d9b-217">String</span></span>|<span data-ttu-id="22d9b-218">请求会议类型： `singleInstance`， `occurence`， `exception`， `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="22d9b-218">The type of requested meeting: `singleInstance`, `occurence`, `exception`, `seriesMaster`.</span></span>|
|<span data-ttu-id="22d9b-219">uniqueBody</span><span class="sxs-lookup"><span data-stu-id="22d9b-219">uniqueBody</span></span>|[<span data-ttu-id="22d9b-220">itemBody</span><span class="sxs-lookup"><span data-stu-id="22d9b-220">itemBody</span></span>](itembody.md)|<span data-ttu-id="22d9b-221">当前邮件专用的邮件正文部分。</span><span class="sxs-lookup"><span data-stu-id="22d9b-221">The part of the body of the message that is unique to the current message.</span></span>|
|<span data-ttu-id="22d9b-222">webLink</span><span class="sxs-lookup"><span data-stu-id="22d9b-222">webLink</span></span>|<span data-ttu-id="22d9b-223">String</span><span class="sxs-lookup"><span data-stu-id="22d9b-223">String</span></span>|<span data-ttu-id="22d9b-224">要在 Outlook Web App 中打开邮件的 URL。</span><span class="sxs-lookup"><span data-stu-id="22d9b-224">The URL to open the message in Outlook Web App.</span></span><br><br><span data-ttu-id="22d9b-p103">可以将 ispopout 参数附加到此 URL 的末尾以更改邮件的显示方式。如果 ispopout 不存在或设置为 1，则邮件显示在弹出窗口中。如果 ispopout 设置为 0，则浏览器将在 Outlook Web App 审阅窗格中显示邮件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p103">You can append an ispopout argument to the end of the URL to change how the message is displayed. If ispopout is not present or if it is set to 1, then the message is shown in a popout window. If ispopout is set to 0, then the browser will show the message in the Outlook Web App review pane.</span></span><br><br><span data-ttu-id="22d9b-p104">如果通过 Outlook Web App 登录邮箱，该邮件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p104">The message will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br><br><span data-ttu-id="22d9b-230">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="22d9b-230">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="22d9b-231">关系</span><span class="sxs-lookup"><span data-stu-id="22d9b-231">Relationships</span></span>
| <span data-ttu-id="22d9b-232">关系</span><span class="sxs-lookup"><span data-stu-id="22d9b-232">Relationship</span></span> | <span data-ttu-id="22d9b-233">类型</span><span class="sxs-lookup"><span data-stu-id="22d9b-233">Type</span></span>   |<span data-ttu-id="22d9b-234">说明</span><span class="sxs-lookup"><span data-stu-id="22d9b-234">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="22d9b-235">attachments</span><span class="sxs-lookup"><span data-stu-id="22d9b-235">attachments</span></span>|<span data-ttu-id="22d9b-236">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22d9b-236">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="22d9b-p105">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p105">Read-only. Nullable.</span></span>|
|<span data-ttu-id="22d9b-239">event</span><span class="sxs-lookup"><span data-stu-id="22d9b-239">event</span></span>|[<span data-ttu-id="22d9b-240">事件</span><span class="sxs-lookup"><span data-stu-id="22d9b-240">Event</span></span>](event.md)| <span data-ttu-id="22d9b-p106">与事件消息相关联的事件。对于与会者或会议室资源，假定已将日历助理设为在会议请求事件消息到达时自动更新包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p106">The event associated with the event message. The assumption for attendees or room resources is that the Calendar Attendant is set to automatically update the calendar with an event when meeting request event messages arrive. Navigation property.  Read-only.</span></span>|
|<span data-ttu-id="22d9b-245">extensions</span><span class="sxs-lookup"><span data-stu-id="22d9b-245">extensions</span></span>|<span data-ttu-id="22d9b-246">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="22d9b-246">[Extension](extension.md) collection</span></span>| <span data-ttu-id="22d9b-p107">只读。可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p107">Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="22d9b-249">方法</span><span class="sxs-lookup"><span data-stu-id="22d9b-249">Methods</span></span>

| <span data-ttu-id="22d9b-250">方法</span><span class="sxs-lookup"><span data-stu-id="22d9b-250">Method</span></span>           | <span data-ttu-id="22d9b-251">返回类型</span><span class="sxs-lookup"><span data-stu-id="22d9b-251">Return Type</span></span>    |<span data-ttu-id="22d9b-252">说明</span><span class="sxs-lookup"><span data-stu-id="22d9b-252">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="22d9b-253">获取 eventMessage</span><span class="sxs-lookup"><span data-stu-id="22d9b-253">Get eventMessage</span></span>](../api/eventmessage-get.md) | [<span data-ttu-id="22d9b-254">eventMessage</span><span class="sxs-lookup"><span data-stu-id="22d9b-254">eventMessage</span></span>](eventmessage.md) |<span data-ttu-id="22d9b-255">读取 eventmessage 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="22d9b-255">Read properties and relationships of eventMessage object.</span></span>|
|[<span data-ttu-id="22d9b-256">创建附件</span><span class="sxs-lookup"><span data-stu-id="22d9b-256">Create Attachment</span></span>](../api/eventmessage-post-attachments.md) |[<span data-ttu-id="22d9b-257">附件</span><span class="sxs-lookup"><span data-stu-id="22d9b-257">Attachment</span></span>](attachment.md)| <span data-ttu-id="22d9b-258">通过发布到附件集合创建新附件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-258">Create a new Attachment by posting to the attachments collection.</span></span>|
|[<span data-ttu-id="22d9b-259">列出附件</span><span class="sxs-lookup"><span data-stu-id="22d9b-259">List attachments</span></span>](../api/eventmessage-list-attachments.md) |<span data-ttu-id="22d9b-260">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="22d9b-260">[Attachment](attachment.md) collection</span></span>| <span data-ttu-id="22d9b-261">获取附件对象集合。</span><span class="sxs-lookup"><span data-stu-id="22d9b-261">Get a Attachment object collection.</span></span>|
|[<span data-ttu-id="22d9b-262">更新</span><span class="sxs-lookup"><span data-stu-id="22d9b-262">Update</span></span>](../api/eventmessage-update.md) | [<span data-ttu-id="22d9b-263">eventMessage</span><span class="sxs-lookup"><span data-stu-id="22d9b-263">eventMessage</span></span>](eventmessage.md)  |<span data-ttu-id="22d9b-264">更新 eventMessage 对象。</span><span class="sxs-lookup"><span data-stu-id="22d9b-264">Update eventMessage object.</span></span> |
|[<span data-ttu-id="22d9b-265">删除</span><span class="sxs-lookup"><span data-stu-id="22d9b-265">Delete</span></span>](../api/eventmessage-delete.md) | <span data-ttu-id="22d9b-266">无</span><span class="sxs-lookup"><span data-stu-id="22d9b-266">None</span></span> |<span data-ttu-id="22d9b-267">更新 eventMessage 对象。</span><span class="sxs-lookup"><span data-stu-id="22d9b-267">Delete eventMessage object.</span></span> |
|[<span data-ttu-id="22d9b-268">复制</span><span class="sxs-lookup"><span data-stu-id="22d9b-268">copy</span></span>](../api/message-copy.md)|[<span data-ttu-id="22d9b-269">邮件</span><span class="sxs-lookup"><span data-stu-id="22d9b-269">Message</span></span>](message.md)||
|[<span data-ttu-id="22d9b-270">createForward</span><span class="sxs-lookup"><span data-stu-id="22d9b-270">createForward</span></span>](../api/message-createforward.md)|[<span data-ttu-id="22d9b-271">邮件</span><span class="sxs-lookup"><span data-stu-id="22d9b-271">Message</span></span>](message.md)||
|[<span data-ttu-id="22d9b-272">createReply</span><span class="sxs-lookup"><span data-stu-id="22d9b-272">createReply</span></span>](../api/message-createreply.md)|[<span data-ttu-id="22d9b-273">邮件</span><span class="sxs-lookup"><span data-stu-id="22d9b-273">Message</span></span>](message.md)||
|[<span data-ttu-id="22d9b-274">createReplyAll</span><span class="sxs-lookup"><span data-stu-id="22d9b-274">createReplyAll</span></span>](../api/message-createreplyall.md)|[<span data-ttu-id="22d9b-275">邮件</span><span class="sxs-lookup"><span data-stu-id="22d9b-275">Message</span></span>](message.md)||
|[<span data-ttu-id="22d9b-276">转发</span><span class="sxs-lookup"><span data-stu-id="22d9b-276">forward</span></span>](../api/message-forward.md)|<span data-ttu-id="22d9b-277">无</span><span class="sxs-lookup"><span data-stu-id="22d9b-277">None</span></span>|<span data-ttu-id="22d9b-278">将邮件转发。</span><span class="sxs-lookup"><span data-stu-id="22d9b-278">Forwards a message.</span></span> <span data-ttu-id="22d9b-279">然后在已发送邮件文件夹中保存邮件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-279">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="22d9b-280">移动</span><span class="sxs-lookup"><span data-stu-id="22d9b-280">move</span></span>](../api/message-move.md)|[<span data-ttu-id="22d9b-281">邮件</span><span class="sxs-lookup"><span data-stu-id="22d9b-281">Message</span></span>](message.md)|<span data-ttu-id="22d9b-282">将邮件移动到 mailFolder。</span><span class="sxs-lookup"><span data-stu-id="22d9b-282">Move the message to a mailFolder.</span></span>|
|[<span data-ttu-id="22d9b-283">回复</span><span class="sxs-lookup"><span data-stu-id="22d9b-283">reply</span></span>](../api/message-reply.md)|<span data-ttu-id="22d9b-284">无</span><span class="sxs-lookup"><span data-stu-id="22d9b-284">None</span></span>|<span data-ttu-id="22d9b-285">消息的发件人的回复。</span><span class="sxs-lookup"><span data-stu-id="22d9b-285">Replys to the sender of a message.</span></span> <span data-ttu-id="22d9b-286">然后在已发送邮件文件夹中保存邮件。</span><span class="sxs-lookup"><span data-stu-id="22d9b-286">The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="22d9b-287">replyAll</span><span class="sxs-lookup"><span data-stu-id="22d9b-287">replyAll</span></span>](../api/message-replyall.md)|<span data-ttu-id="22d9b-288">无</span><span class="sxs-lookup"><span data-stu-id="22d9b-288">None</span></span>|<span data-ttu-id="22d9b-p110">答复邮件的所有收件人。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p110">Reply to all recipients of a message. The message is then saved in the Sent Items folder.</span></span>|
|[<span data-ttu-id="22d9b-291">发送</span><span class="sxs-lookup"><span data-stu-id="22d9b-291">send</span></span>](../api/message-send.md)|<span data-ttu-id="22d9b-292">无</span><span class="sxs-lookup"><span data-stu-id="22d9b-292">None</span></span>|<span data-ttu-id="22d9b-p111">发送以前创建的邮件草稿。然后邮件保存在已发送邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="22d9b-p111">Sends a previously created message draft. The message is then saved in the Sent Items folder.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "eventMessageRequest resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
