---
title: 事件资源类型
description: 日历中的事件。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 64e8c449f5336b06da8287aa057fb4ad7776812e
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193300"
---
# <a name="event-resource-type"></a><span data-ttu-id="c9f5b-103">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="c9f5b-103">event resource type</span></span>

<span data-ttu-id="c9f5b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c9f5b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c9f5b-105">[用户](user.md)日历或 Microsoft 365 [组](group.md)默认日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-105">An event in a [user](user.md) calendar, or the default calendar of a Microsoft 365 [group](group.md).</span></span>

<span data-ttu-id="c9f5b-106">**事件**中包含的最大与会者人数，以及发送自 Exchange Online 邮箱的 [eventMessage](eventmessage.md) 中的收件人数上限都是 500 人。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-106">The maximum number of attendees included in an **event**, and the maximum number of recipients in an [eventMessage](eventmessage.md) sent from an Exchange Online mailbox is 500.</span></span> <span data-ttu-id="c9f5b-107">有关详细信息，请参阅[发送限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-107">For more information, see [sending limits](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).</span></span>

<span data-ttu-id="c9f5b-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="c9f5b-108">This resource supports:</span></span>

- <span data-ttu-id="c9f5b-109">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="c9f5b-110">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="c9f5b-111">通过提供 [delta](../api/event-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>

> <span data-ttu-id="c9f5b-112">**注释：** 与用户日历、组日历及其事件交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="c9f5b-112">**Note:** There are a few minor differences in the way you can interact with user calendars, group calendars, and their events:</span></span>

- <span data-ttu-id="c9f5b-113">只可以组织 [calendarGroup](calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-113">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="c9f5b-114">只能将 [attachment](attachment.md) 对象添加到用户日历中的事件，而不能添加到组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-114">You can add [attachment](attachment.md) objects to events in only user calendars, but not to events in group calendars.</span></span>
- <span data-ttu-id="c9f5b-115">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-115">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="c9f5b-116">只可以[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)_用户_日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-116">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for _user_ calendars only.</span></span>
- <span data-ttu-id="c9f5b-117">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-117">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="c9f5b-118">只可以[暂停](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)_用户_日历中的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-118">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for _user_ calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="c9f5b-119">方法</span><span class="sxs-lookup"><span data-stu-id="c9f5b-119">Methods</span></span>

| <span data-ttu-id="c9f5b-120">方法</span><span class="sxs-lookup"><span data-stu-id="c9f5b-120">Method</span></span>       | <span data-ttu-id="c9f5b-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="c9f5b-121">Return Type</span></span>  |<span data-ttu-id="c9f5b-122">说明</span><span class="sxs-lookup"><span data-stu-id="c9f5b-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="c9f5b-123">列出事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-123">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="c9f5b-124">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-124">[event](event.md) collection</span></span> |<span data-ttu-id="c9f5b-p104">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p104">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="c9f5b-127">创建事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-127">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="c9f5b-128">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-128">event</span></span>](event.md)| <span data-ttu-id="c9f5b-129">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-129">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="c9f5b-130">获取事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-130">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="c9f5b-131">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-131">event</span></span>](event.md) |<span data-ttu-id="c9f5b-132">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-132">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="c9f5b-133">更新</span><span class="sxs-lookup"><span data-stu-id="c9f5b-133">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="c9f5b-134">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-134">event</span></span>](event.md) |<span data-ttu-id="c9f5b-135">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-135">Update event object.</span></span> |
|[<span data-ttu-id="c9f5b-136">删除</span><span class="sxs-lookup"><span data-stu-id="c9f5b-136">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="c9f5b-137">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-137">None</span></span> |<span data-ttu-id="c9f5b-138">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-138">Delete event object.</span></span> |
|[<span data-ttu-id="c9f5b-139">接受</span><span class="sxs-lookup"><span data-stu-id="c9f5b-139">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="c9f5b-140">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-140">None</span></span>|<span data-ttu-id="c9f5b-141">接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-141">Accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="c9f5b-142">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="c9f5b-142">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="c9f5b-143">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-143">None</span></span>|<span data-ttu-id="c9f5b-144">暂时接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-144">Tentatively accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="c9f5b-145">拒绝</span><span class="sxs-lookup"><span data-stu-id="c9f5b-145">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="c9f5b-146">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-146">None</span></span>|<span data-ttu-id="c9f5b-147">拒绝用户日历中的指定事件邀请。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-147">Decline invitation to the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="c9f5b-148">delta</span><span class="sxs-lookup"><span data-stu-id="c9f5b-148">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="c9f5b-149">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-149">[event](event.md) collection</span></span>|<span data-ttu-id="c9f5b-150">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-150">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="c9f5b-151">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="c9f5b-151">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="c9f5b-152">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-152">None</span></span>|<span data-ttu-id="c9f5b-153">消除用户日历中指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-153">Dismiss the reminder for the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="c9f5b-154">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="c9f5b-154">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="c9f5b-155">无</span><span class="sxs-lookup"><span data-stu-id="c9f5b-155">None</span></span>|<span data-ttu-id="c9f5b-156">将用户日历中指定事件的提醒推迟至新的时间。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-156">Postpone a reminder for the specified event in a user calendar until a new time.</span></span>|
|[<span data-ttu-id="c9f5b-157">列出实例</span><span class="sxs-lookup"><span data-stu-id="c9f5b-157">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="c9f5b-158">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-158">[event](event.md) collection</span></span>| <span data-ttu-id="c9f5b-p105">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p105">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="c9f5b-161">**附件**</span><span class="sxs-lookup"><span data-stu-id="c9f5b-161">**Attachments**</span></span>| | |
|[<span data-ttu-id="c9f5b-162">列出附件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-162">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="c9f5b-163">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-163">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="c9f5b-164">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-164">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="c9f5b-165">Add attachment</span><span class="sxs-lookup"><span data-stu-id="c9f5b-165">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="c9f5b-166">attachment</span><span class="sxs-lookup"><span data-stu-id="c9f5b-166">attachment</span></span>](attachment.md)| <span data-ttu-id="c9f5b-167">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-167">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="c9f5b-168">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="c9f5b-168">**Open extensions**</span></span>| | |
|[<span data-ttu-id="c9f5b-169">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="c9f5b-169">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="c9f5b-170">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="c9f5b-170">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="c9f5b-171">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-171">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="c9f5b-172">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="c9f5b-172">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="c9f5b-173">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-173">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="c9f5b-174">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-174">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="c9f5b-175">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="c9f5b-175">**Extended properties**</span></span>| | |
|[<span data-ttu-id="c9f5b-176">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="c9f5b-176">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="c9f5b-177">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-177">event</span></span>](event.md)  |<span data-ttu-id="c9f5b-178">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-178">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="c9f5b-179">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-179">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="c9f5b-180">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-180">event</span></span>](event.md) | <span data-ttu-id="c9f5b-181">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-181">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="c9f5b-182">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="c9f5b-182">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="c9f5b-183">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-183">event</span></span>](event.md) | <span data-ttu-id="c9f5b-184">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-184">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="c9f5b-185">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-185">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="c9f5b-186">事件</span><span class="sxs-lookup"><span data-stu-id="c9f5b-186">event</span></span>](event.md) | <span data-ttu-id="c9f5b-187">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-187">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="c9f5b-188">属性</span><span class="sxs-lookup"><span data-stu-id="c9f5b-188">Properties</span></span>
| <span data-ttu-id="c9f5b-189">属性</span><span class="sxs-lookup"><span data-stu-id="c9f5b-189">Property</span></span>     | <span data-ttu-id="c9f5b-190">类型</span><span class="sxs-lookup"><span data-stu-id="c9f5b-190">Type</span></span>   |<span data-ttu-id="c9f5b-191">说明</span><span class="sxs-lookup"><span data-stu-id="c9f5b-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9f5b-192">allowNewTimeProposals</span><span class="sxs-lookup"><span data-stu-id="c9f5b-192">allowNewTimeProposals</span></span>| <span data-ttu-id="c9f5b-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="c9f5b-193">Boolean</span></span> | <span data-ttu-id="c9f5b-194">如果会议组织者允许被邀请者在响应时建议新时间，则为`True`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-194">`True` if the meeting organizer allows invitees to propose a new time when responding, `false` otherwise.</span></span> <span data-ttu-id="c9f5b-195">可选。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-195">Optional.</span></span> <span data-ttu-id="c9f5b-196">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-196">Default is `true`.</span></span> |
|<span data-ttu-id="c9f5b-197">attendees</span><span class="sxs-lookup"><span data-stu-id="c9f5b-197">attendees</span></span>|<span data-ttu-id="c9f5b-198">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-198">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="c9f5b-199">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-199">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="c9f5b-200">body</span><span class="sxs-lookup"><span data-stu-id="c9f5b-200">body</span></span>|[<span data-ttu-id="c9f5b-201">itemBody</span><span class="sxs-lookup"><span data-stu-id="c9f5b-201">itemBody</span></span>](itembody.md)|<span data-ttu-id="c9f5b-p107">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p107">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="c9f5b-204">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="c9f5b-204">bodyPreview</span></span>|<span data-ttu-id="c9f5b-205">字符串</span><span class="sxs-lookup"><span data-stu-id="c9f5b-205">String</span></span>|<span data-ttu-id="c9f5b-p108">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p108">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="c9f5b-208">categories</span><span class="sxs-lookup"><span data-stu-id="c9f5b-208">categories</span></span>|<span data-ttu-id="c9f5b-209">String collection</span><span class="sxs-lookup"><span data-stu-id="c9f5b-209">String collection</span></span>|<span data-ttu-id="c9f5b-210">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-210">The categories associated with the event.</span></span>|
|<span data-ttu-id="c9f5b-211">changeKey</span><span class="sxs-lookup"><span data-stu-id="c9f5b-211">changeKey</span></span>|<span data-ttu-id="c9f5b-212">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-212">String</span></span>|<span data-ttu-id="c9f5b-p109">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p109">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="c9f5b-216">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9f5b-216">createdDateTime</span></span>|<span data-ttu-id="c9f5b-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9f5b-217">DateTimeOffset</span></span>|<span data-ttu-id="c9f5b-p110">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p110">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9f5b-220">end</span><span class="sxs-lookup"><span data-stu-id="c9f5b-220">end</span></span>|[<span data-ttu-id="c9f5b-221">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9f5b-221">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="c9f5b-222">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-222">The date, time, and time zone that the event ends.</span></span> <span data-ttu-id="c9f5b-223">默认情况下，结束时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-223">By default, the end time is in UTC.</span></span>|
|<span data-ttu-id="c9f5b-224">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="c9f5b-224">hasAttachments</span></span>|<span data-ttu-id="c9f5b-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-225">Boolean</span></span>|<span data-ttu-id="c9f5b-226">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-226">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="c9f5b-227">iCalUId</span><span class="sxs-lookup"><span data-stu-id="c9f5b-227">iCalUId</span></span>|<span data-ttu-id="c9f5b-228">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-228">String</span></span>|<span data-ttu-id="c9f5b-229">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-229">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="c9f5b-230">只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-230">Read-only.</span></span>|
|<span data-ttu-id="c9f5b-231">id</span><span class="sxs-lookup"><span data-stu-id="c9f5b-231">id</span></span>|<span data-ttu-id="c9f5b-232">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-232">String</span></span>| <span data-ttu-id="c9f5b-233">只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-233">Read-only.</span></span>|
|<span data-ttu-id="c9f5b-234">importance</span><span class="sxs-lookup"><span data-stu-id="c9f5b-234">importance</span></span>|<span data-ttu-id="c9f5b-235">importance</span><span class="sxs-lookup"><span data-stu-id="c9f5b-235">importance</span></span>|<span data-ttu-id="c9f5b-236">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-236">The importance of the event.</span></span> <span data-ttu-id="c9f5b-237">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-237">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="c9f5b-238">isAllDay</span><span class="sxs-lookup"><span data-stu-id="c9f5b-238">isAllDay</span></span>|<span data-ttu-id="c9f5b-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-239">Boolean</span></span>|<span data-ttu-id="c9f5b-240">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-240">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="c9f5b-241">isCancelled</span><span class="sxs-lookup"><span data-stu-id="c9f5b-241">isCancelled</span></span>|<span data-ttu-id="c9f5b-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-242">Boolean</span></span>|<span data-ttu-id="c9f5b-243">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-243">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="c9f5b-244">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="c9f5b-244">isOnlineMeeting</span></span>|<span data-ttu-id="c9f5b-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-245">Boolean</span></span>| <span data-ttu-id="c9f5b-246">若此事件包含联机会议信息则为 `True`，反之则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-246">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="c9f5b-247">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-247">Default is false.</span></span> <span data-ttu-id="c9f5b-248">可选。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-248">Optional.</span></span>|
|<span data-ttu-id="c9f5b-249">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="c9f5b-249">isOrganizer</span></span>|<span data-ttu-id="c9f5b-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-250">Boolean</span></span>|<span data-ttu-id="c9f5b-251">如果日历所有者（通过“[日历](calendar.md)”的“**所有者**”属性指定）是事件的组织者（通过“**事件**”的“**组织者**”属性指定），设定为 true。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-251">Set to true if the calendar owner (specified by the **owner** property of the [calendar](calendar.md)) is the organizer of the event (specified by the **organizer** property of the **event**).</span></span> <span data-ttu-id="c9f5b-252">这也适用于代理人代表所有者组织事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-252">This also applies if a delegate organized the event on behalf of the owner.</span></span>|
|<span data-ttu-id="c9f5b-253">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="c9f5b-253">isReminderOn</span></span>|<span data-ttu-id="c9f5b-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9f5b-254">Boolean</span></span>|<span data-ttu-id="c9f5b-255">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-255">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="c9f5b-256">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9f5b-256">lastModifiedDateTime</span></span>|<span data-ttu-id="c9f5b-257">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9f5b-257">DateTimeOffset</span></span>|<span data-ttu-id="c9f5b-p116">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9f5b-260">location</span><span class="sxs-lookup"><span data-stu-id="c9f5b-260">location</span></span>|[<span data-ttu-id="c9f5b-261">位置</span><span class="sxs-lookup"><span data-stu-id="c9f5b-261">location</span></span>](location.md)|<span data-ttu-id="c9f5b-262">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-262">The location of the event.</span></span>|
|<span data-ttu-id="c9f5b-263">locations</span><span class="sxs-lookup"><span data-stu-id="c9f5b-263">locations</span></span>|<span data-ttu-id="c9f5b-264">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-264">[location](location.md) collection</span></span>|<span data-ttu-id="c9f5b-265">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-265">The locations where the event is held or attended from.</span></span> <span data-ttu-id="c9f5b-266">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-266">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="c9f5b-267">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-267">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="c9f5b-268">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="c9f5b-268">onlineMeeting</span></span>|[<span data-ttu-id="c9f5b-269">OnlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="c9f5b-269">OnlineMeetingInfo</span></span>](onlinemeetinginfo.md)| <span data-ttu-id="c9f5b-270">关于与会者如何加入联机会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-270">Details for an attendee to join the meeting online.</span></span> <span data-ttu-id="c9f5b-271">只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-271">Read-only.</span></span>|
|<span data-ttu-id="c9f5b-272">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="c9f5b-272">onlineMeetingProvider</span></span>|<span data-ttu-id="c9f5b-273">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="c9f5b-273">onlineMeetingProviderType</span></span>| <span data-ttu-id="c9f5b-274">表示联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-274">Represents the online meeting service provider.</span></span> <span data-ttu-id="c9f5b-275">可取值为：`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-275">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="c9f5b-276">可选。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-276">Optional.</span></span> |
|<span data-ttu-id="c9f5b-277">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="c9f5b-277">onlineMeetingUrl</span></span>|<span data-ttu-id="c9f5b-278">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-278">String</span></span>|<span data-ttu-id="c9f5b-279">联机会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-279">A URL for an online meeting.</span></span> <span data-ttu-id="c9f5b-280">仅当组织者将事件指定为联机会议（如 Skype 会议）时才会设置此属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-280">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="c9f5b-281">只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-281">Read-only.</span></span>|
|<span data-ttu-id="c9f5b-282">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="c9f5b-282">organizer</span></span>|[<span data-ttu-id="c9f5b-283">recipient</span><span class="sxs-lookup"><span data-stu-id="c9f5b-283">recipient</span></span>](recipient.md)|<span data-ttu-id="c9f5b-284">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-284">The organizer of the event.</span></span>|
|<span data-ttu-id="c9f5b-285">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9f5b-285">originalEndTimeZone</span></span>|<span data-ttu-id="c9f5b-286">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-286">String</span></span>|<span data-ttu-id="c9f5b-287">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-287">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="c9f5b-288">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-288">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="c9f5b-289">originalStart</span><span class="sxs-lookup"><span data-stu-id="c9f5b-289">originalStart</span></span>|<span data-ttu-id="c9f5b-290">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9f5b-290">DateTimeOffset</span></span>|<span data-ttu-id="c9f5b-p122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9f5b-293">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9f5b-293">originalStartTimeZone</span></span>|<span data-ttu-id="c9f5b-294">字符串</span><span class="sxs-lookup"><span data-stu-id="c9f5b-294">String</span></span>|<span data-ttu-id="c9f5b-p123">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p123">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="c9f5b-297">recurrence</span><span class="sxs-lookup"><span data-stu-id="c9f5b-297">recurrence</span></span>|[<span data-ttu-id="c9f5b-298">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="c9f5b-298">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="c9f5b-299">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-299">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="c9f5b-300">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="c9f5b-300">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="c9f5b-301">Int32</span><span class="sxs-lookup"><span data-stu-id="c9f5b-301">Int32</span></span>|<span data-ttu-id="c9f5b-302">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-302">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="c9f5b-303">responseRequested</span><span class="sxs-lookup"><span data-stu-id="c9f5b-303">responseRequested</span></span>|<span data-ttu-id="c9f5b-304">布尔值</span><span class="sxs-lookup"><span data-stu-id="c9f5b-304">Boolean</span></span>|<span data-ttu-id="c9f5b-305">默认值为 true，表示组织者愿意被邀请者发送事件响应。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-305">Default is true, which represents the organizer would like an invitee to send a response to the event.</span></span>|
|<span data-ttu-id="c9f5b-306">responseStatus</span><span class="sxs-lookup"><span data-stu-id="c9f5b-306">responseStatus</span></span>|[<span data-ttu-id="c9f5b-307">responseStatus</span><span class="sxs-lookup"><span data-stu-id="c9f5b-307">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="c9f5b-308">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-308">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="c9f5b-309">sensitivity</span><span class="sxs-lookup"><span data-stu-id="c9f5b-309">sensitivity</span></span>|<span data-ttu-id="c9f5b-310">敏感度</span><span class="sxs-lookup"><span data-stu-id="c9f5b-310">sensitivity</span></span>| <span data-ttu-id="c9f5b-311">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-311">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="c9f5b-312">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="c9f5b-312">seriesMasterId</span></span>|<span data-ttu-id="c9f5b-313">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-313">String</span></span>|<span data-ttu-id="c9f5b-314">定期系列主项的 ID（如果此事件是定期系列的一部分）。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-314">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="c9f5b-315">showAs</span><span class="sxs-lookup"><span data-stu-id="c9f5b-315">showAs</span></span>|<span data-ttu-id="c9f5b-316">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="c9f5b-316">freeBusyStatus</span></span>|<span data-ttu-id="c9f5b-317">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-317">The status to show.</span></span> <span data-ttu-id="c9f5b-318">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-318">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="c9f5b-319">start</span><span class="sxs-lookup"><span data-stu-id="c9f5b-319">start</span></span>|[<span data-ttu-id="c9f5b-320">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="c9f5b-320">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="c9f5b-321">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-321">The date, time, and time zone that the event starts.</span></span> <span data-ttu-id="c9f5b-322">默认情况下，开始时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-322">By default, the start time is in UTC.</span></span>|
|<span data-ttu-id="c9f5b-323">subject</span><span class="sxs-lookup"><span data-stu-id="c9f5b-323">subject</span></span>|<span data-ttu-id="c9f5b-324">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-324">String</span></span>|<span data-ttu-id="c9f5b-325">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-325">The text of the event's subject line.</span></span>|
|<span data-ttu-id="c9f5b-326">transactionId</span><span class="sxs-lookup"><span data-stu-id="c9f5b-326">transactionId</span></span> |<span data-ttu-id="c9f5b-327">字符串</span><span class="sxs-lookup"><span data-stu-id="c9f5b-327">String</span></span> |<span data-ttu-id="c9f5b-328">客户端应用为服务器指定的自定义标识符，用于避免因客户端重试创建相同事件而导致冗余的 POST 操作。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-328">A custom identifier specified by a client app for the server to avoid redundant POST operations in case of client retries to create the same event.</span></span> <span data-ttu-id="c9f5b-329">当低网络连接性导致客户端在从服务器中收到客户端先前创建事件请求的响应之前超时时，此功能很有用。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-329">This is useful when low network connectivity causes the client to time out before receiving a response from the server for the client's prior create-event request.</span></span> <span data-ttu-id="c9f5b-330">你在创建事件时设置 **transactionId**，之后不能在后续更新中更改 **transactionId**。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-330">After you set **transactionId** when creating an event, you cannot change **transactionId** in a subsequent update.</span></span> <span data-ttu-id="c9f5b-331">如果应用已设置此属性，则仅在响应有效负载中返回此属性。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-331">This property is only returned in a response payload if an app has set it.</span></span> <span data-ttu-id="c9f5b-332">可选。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-332">Optional.</span></span>|
|<span data-ttu-id="c9f5b-333">type</span><span class="sxs-lookup"><span data-stu-id="c9f5b-333">type</span></span>|<span data-ttu-id="c9f5b-334">eventType</span><span class="sxs-lookup"><span data-stu-id="c9f5b-334">eventType</span></span>|<span data-ttu-id="c9f5b-335">事件类型。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-335">The event type.</span></span> <span data-ttu-id="c9f5b-336">可能的值包括 `singleInstance`、`occurrence`、`exception`、`seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-336">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="c9f5b-337">只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-337">Read-only.</span></span>|
|<span data-ttu-id="c9f5b-338">webLink</span><span class="sxs-lookup"><span data-stu-id="c9f5b-338">webLink</span></span>|<span data-ttu-id="c9f5b-339">String</span><span class="sxs-lookup"><span data-stu-id="c9f5b-339">String</span></span>|<span data-ttu-id="c9f5b-340">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-340">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="c9f5b-341">如果登录邮件，则 Outlook 网页面会在浏览器中打开事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-341">Outlook on the web opens the event in the browser if you are signed in to your mailbox.</span></span> <span data-ttu-id="c9f5b-342">否则，Outlook 网页面会提示你进行登录。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-342">Otherwise, Outlook on the web prompts you to sign in.</span></span><br/><br/><span data-ttu-id="c9f5b-343">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-343">This URL can be accessed from within an iFrame.</span></span>|

> [!NOTE]
> <span data-ttu-id="c9f5b-344">**webLink** 属性指定了一个 URL，它仅在 Outlook 网页版早期版本中打开事件。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-344">The **webLink** property specifies a URL that opens the event in only earlier versions of Outlook on the web.</span></span> <span data-ttu-id="c9f5b-345">以下是 URL 格式，其中 _{event-id}_ 是 **id** 属性的 _**URL 编码**_ 值：</span><span class="sxs-lookup"><span data-stu-id="c9f5b-345">The following are the URL formats, with _{event-id}_ being the _**URL-encoded**_ value of the **id** property:</span></span>
>
> * <span data-ttu-id="c9f5b-346">对于工作或学校帐户：`https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-346">For work or school accounts: `https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> * <span data-ttu-id="c9f5b-347">对于 Microsoft 帐户：`https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-347">For Microsoft accounts: `https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> <span data-ttu-id="c9f5b-348">要在 Outlook 网页版的当前版本中打开事件，请将 URL 转换为下述格式之一，并使用该 URL 打开事件：</span><span class="sxs-lookup"><span data-stu-id="c9f5b-348">To open the event in a current version of Outlook on the web, convert the URL to one of the following formats, and use that URL to open the event:</span></span>
>
> * <span data-ttu-id="c9f5b-349">对于工作或学校帐户：`https://outlook.office365.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-349">For work or school accounts: `https://outlook.office365.com/calendar/item/{event-id}`</span></span>
>
> * <span data-ttu-id="c9f5b-350">对于 Microsoft 帐户：`https://outlook.live.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="c9f5b-350">For Microsoft accounts: `https://outlook.live.com/calendar/item/{event-id}`</span></span>


## <a name="relationships"></a><span data-ttu-id="c9f5b-351">关系</span><span class="sxs-lookup"><span data-stu-id="c9f5b-351">Relationships</span></span>
| <span data-ttu-id="c9f5b-352">关系</span><span class="sxs-lookup"><span data-stu-id="c9f5b-352">Relationship</span></span> | <span data-ttu-id="c9f5b-353">类型</span><span class="sxs-lookup"><span data-stu-id="c9f5b-353">Type</span></span>   |<span data-ttu-id="c9f5b-354">说明</span><span class="sxs-lookup"><span data-stu-id="c9f5b-354">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9f5b-355">attachments</span><span class="sxs-lookup"><span data-stu-id="c9f5b-355">attachments</span></span>|<span data-ttu-id="c9f5b-356">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-356">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="c9f5b-p130">事件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p130">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c9f5b-361">日历</span><span class="sxs-lookup"><span data-stu-id="c9f5b-361">calendar</span></span>|[<span data-ttu-id="c9f5b-362">日历</span><span class="sxs-lookup"><span data-stu-id="c9f5b-362">calendar</span></span>](calendar.md)|<span data-ttu-id="c9f5b-p131">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p131">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="c9f5b-366">extensions</span><span class="sxs-lookup"><span data-stu-id="c9f5b-366">extensions</span></span>|<span data-ttu-id="c9f5b-367">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-367">[Extension](extension.md) collection</span></span>|<span data-ttu-id="c9f5b-p132">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p132">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c9f5b-371">instances</span><span class="sxs-lookup"><span data-stu-id="c9f5b-371">instances</span></span>|<span data-ttu-id="c9f5b-372">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-372">[event](event.md) collection</span></span>|<span data-ttu-id="c9f5b-p133">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p133">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c9f5b-377">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c9f5b-377">multiValueExtendedProperties</span></span>|<span data-ttu-id="c9f5b-378">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c9f5b-378">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c9f5b-p134">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p134">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="c9f5b-382">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="c9f5b-382">singleValueExtendedProperties</span></span>|<span data-ttu-id="c9f5b-383">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="c9f5b-383">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="c9f5b-p135">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-p135">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c9f5b-387">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9f5b-387">JSON representation</span></span>

<span data-ttu-id="c9f5b-388">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9f5b-388">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "attachments",
    "calendar",
    "extensions",
    "instances",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.outlookItem",
  "@odata.type": "microsoft.graph.event",
  "@odata.annotations": [
    {
      "property": "attachments",
      "capabilities": {
        "changeTracking": false,
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "calendar",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "instances",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    }
  ]
}-->

```json
{
  "allowNewTimeProposals": "Boolean",
  "attendees": [{"@odata.type": "microsoft.graph.attendee"}],
  "body": {"@odata.type": "microsoft.graph.itemBody"},
  "bodyPreview": "string",
  "categories": ["string"],
  "changeKey": "string",
  "createdDateTime": "String (timestamp)",
  "end": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "hasAttachments": true,
  "iCalUId": "string",
  "id": "string (identifier)",
  "importance": "String",
  "isAllDay": true,
  "isCancelled": true,
  "isOnlineMeeting": true,
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
  "onlineMeeting": {"@odata.type": "microsoft.graph.onlineMeetingInfo"},
  "onlineMeetingProvider": "string",
  "onlineMeetingUrl": "string",
  "organizer": {"@odata.type": "microsoft.graph.recipient"},
  "originalEndTimeZone": "string",
  "originalStart": "String (timestamp)",
  "originalStartTimeZone": "string",
  "recurrence": {"@odata.type": "microsoft.graph.patternedRecurrence"},
  "reminderMinutesBeforeStart": 1024,
  "responseRequested": true,
  "responseStatus": {"@odata.type": "microsoft.graph.responseStatus"},
  "sensitivity": "String",
  "seriesMasterId": "string",
  "showAs": "String",
  "start": {"@odata.type": "microsoft.graph.dateTimeTimeZone"},
  "subject": "string",
  "transactionId": "string",
  "type": "String",
  "webLink": "string",

  "attachments": [ { "@odata.type": "microsoft.graph.attachment" } ],
  "calendar": { "@odata.type": "microsoft.graph.calendar" },
  "extensions": [ { "@odata.type": "microsoft.graph.extension" } ],
  "instances": [ { "@odata.type": "microsoft.graph.event" }],
  "multiValueExtendedProperties": [ { "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty" }],
  "singleValueExtendedProperties": [ { "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty" }]

}

```


## <a name="see-also"></a><span data-ttu-id="c9f5b-389">另请参阅</span><span class="sxs-lookup"><span data-stu-id="c9f5b-389">See also</span></span>

- [<span data-ttu-id="c9f5b-390">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="c9f5b-390">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="c9f5b-391">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="c9f5b-391">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="c9f5b-392">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c9f5b-392">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="c9f5b-393">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c9f5b-393">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="c9f5b-394">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="c9f5b-394">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

