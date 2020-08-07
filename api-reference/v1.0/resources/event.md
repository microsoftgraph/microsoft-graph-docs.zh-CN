---
title: 事件资源类型
description: 日历中的事件。
author: harini84
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: d0d39fd4ed4a905f66cc223b8832e42bbda676a4
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565925"
---
# <a name="event-resource-type"></a><span data-ttu-id="f4c6f-103">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="f4c6f-103">event resource type</span></span>

<span data-ttu-id="f4c6f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4c6f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f4c6f-105">[用户](user.md)日历或 Microsoft 365 [组](group.md)默认日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-105">An event in a [user](user.md) calendar, or the default calendar of a Microsoft 365 [group](group.md).</span></span>

<span data-ttu-id="f4c6f-106">**事件**中包含的最大与会者人数，以及发送自 Exchange Online 邮箱的 [eventMessage](eventmessage.md) 中的收件人数上限都是 500 人。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-106">The maximum number of attendees included in an **event**, and the maximum number of recipients in an [eventMessage](eventmessage.md) sent from an Exchange Online mailbox is 500.</span></span> <span data-ttu-id="f4c6f-107">有关详细信息，请参阅[发送限制](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-107">For more information, see [sending limits](/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).</span></span>

<span data-ttu-id="f4c6f-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="f4c6f-108">This resource supports:</span></span>

- <span data-ttu-id="f4c6f-109">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="f4c6f-110">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="f4c6f-111">通过提供 [delta](../api/event-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>

> <span data-ttu-id="f4c6f-112">**注释：** 与用户日历、组日历及其事件交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="f4c6f-112">**Note:** There are a few minor differences in the way you can interact with user calendars, group calendars, and their events:</span></span>

- <span data-ttu-id="f4c6f-113">只可以组织 [calendarGroup](calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-113">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="f4c6f-114">只能将 [attachment](attachment.md) 对象添加到用户日历中的事件，而不能添加到组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-114">You can add [attachment](attachment.md) objects to events in only user calendars, but not to events in group calendars.</span></span>
- <span data-ttu-id="f4c6f-115">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-115">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="f4c6f-116">只可以[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)_用户_日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-116">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for _user_ calendars only.</span></span>
- <span data-ttu-id="f4c6f-117">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-117">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="f4c6f-118">只可以[暂停](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)_用户_日历中的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-118">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for _user_ calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="f4c6f-119">方法</span><span class="sxs-lookup"><span data-stu-id="f4c6f-119">Methods</span></span>

| <span data-ttu-id="f4c6f-120">方法</span><span class="sxs-lookup"><span data-stu-id="f4c6f-120">Method</span></span>       | <span data-ttu-id="f4c6f-121">返回类型</span><span class="sxs-lookup"><span data-stu-id="f4c6f-121">Return Type</span></span>  |<span data-ttu-id="f4c6f-122">说明</span><span class="sxs-lookup"><span data-stu-id="f4c6f-122">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f4c6f-123">列出事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-123">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="f4c6f-124">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-124">[event](event.md) collection</span></span> |<span data-ttu-id="f4c6f-p104">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p104">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="f4c6f-127">创建事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-127">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="f4c6f-128">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-128">event</span></span>](event.md)| <span data-ttu-id="f4c6f-129">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-129">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="f4c6f-130">获取事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-130">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="f4c6f-131">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-131">event</span></span>](event.md) |<span data-ttu-id="f4c6f-132">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-132">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="f4c6f-133">更新</span><span class="sxs-lookup"><span data-stu-id="f4c6f-133">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="f4c6f-134">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-134">event</span></span>](event.md) |<span data-ttu-id="f4c6f-135">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-135">Update event object.</span></span> |
|[<span data-ttu-id="f4c6f-136">删除</span><span class="sxs-lookup"><span data-stu-id="f4c6f-136">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="f4c6f-137">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-137">None</span></span> |<span data-ttu-id="f4c6f-138">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-138">Delete event object.</span></span> |
|[<span data-ttu-id="f4c6f-139">接受</span><span class="sxs-lookup"><span data-stu-id="f4c6f-139">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="f4c6f-140">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-140">None</span></span>|<span data-ttu-id="f4c6f-141">接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-141">Accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="f4c6f-142">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="f4c6f-142">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="f4c6f-143">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-143">None</span></span>|<span data-ttu-id="f4c6f-144">暂时接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-144">Tentatively accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="f4c6f-145">拒绝</span><span class="sxs-lookup"><span data-stu-id="f4c6f-145">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="f4c6f-146">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-146">None</span></span>|<span data-ttu-id="f4c6f-147">拒绝用户日历中的指定事件邀请。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-147">Decline invitation to the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="f4c6f-148">delta</span><span class="sxs-lookup"><span data-stu-id="f4c6f-148">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="f4c6f-149">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-149">[event](event.md) collection</span></span>|<span data-ttu-id="f4c6f-150">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-150">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="f4c6f-151">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="f4c6f-151">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="f4c6f-152">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-152">None</span></span>|<span data-ttu-id="f4c6f-153">消除用户日历中指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-153">Dismiss the reminder for the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="f4c6f-154">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="f4c6f-154">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="f4c6f-155">无</span><span class="sxs-lookup"><span data-stu-id="f4c6f-155">None</span></span>|<span data-ttu-id="f4c6f-156">将用户日历中指定事件的提醒推迟至新的时间。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-156">Postpone a reminder for the specified event in a user calendar until a new time.</span></span>|
|[<span data-ttu-id="f4c6f-157">列出实例</span><span class="sxs-lookup"><span data-stu-id="f4c6f-157">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="f4c6f-158">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-158">[event](event.md) collection</span></span>| <span data-ttu-id="f4c6f-p105">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p105">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="f4c6f-161">**附件**</span><span class="sxs-lookup"><span data-stu-id="f4c6f-161">**Attachments**</span></span>| | |
|[<span data-ttu-id="f4c6f-162">列出附件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-162">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="f4c6f-163">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-163">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="f4c6f-164">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-164">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="f4c6f-165">Add attachment</span><span class="sxs-lookup"><span data-stu-id="f4c6f-165">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="f4c6f-166">attachment</span><span class="sxs-lookup"><span data-stu-id="f4c6f-166">attachment</span></span>](attachment.md)| <span data-ttu-id="f4c6f-167">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-167">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="f4c6f-168">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="f4c6f-168">**Open extensions**</span></span>| | |
|[<span data-ttu-id="f4c6f-169">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="f4c6f-169">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="f4c6f-170">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="f4c6f-170">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="f4c6f-171">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-171">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="f4c6f-172">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="f4c6f-172">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="f4c6f-173">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-173">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="f4c6f-174">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-174">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="f4c6f-175">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="f4c6f-175">**Extended properties**</span></span>| | |
|[<span data-ttu-id="f4c6f-176">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="f4c6f-176">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="f4c6f-177">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-177">event</span></span>](event.md)  |<span data-ttu-id="f4c6f-178">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-178">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="f4c6f-179">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-179">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f4c6f-180">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-180">event</span></span>](event.md) | <span data-ttu-id="f4c6f-181">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-181">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="f4c6f-182">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="f4c6f-182">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="f4c6f-183">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-183">event</span></span>](event.md) | <span data-ttu-id="f4c6f-184">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-184">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="f4c6f-185">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-185">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="f4c6f-186">事件</span><span class="sxs-lookup"><span data-stu-id="f4c6f-186">event</span></span>](event.md) | <span data-ttu-id="f4c6f-187">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-187">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="f4c6f-188">属性</span><span class="sxs-lookup"><span data-stu-id="f4c6f-188">Properties</span></span>
| <span data-ttu-id="f4c6f-189">属性</span><span class="sxs-lookup"><span data-stu-id="f4c6f-189">Property</span></span>     | <span data-ttu-id="f4c6f-190">类型</span><span class="sxs-lookup"><span data-stu-id="f4c6f-190">Type</span></span>   |<span data-ttu-id="f4c6f-191">说明</span><span class="sxs-lookup"><span data-stu-id="f4c6f-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c6f-192">allowNewTimeProposals</span><span class="sxs-lookup"><span data-stu-id="f4c6f-192">allowNewTimeProposals</span></span>| <span data-ttu-id="f4c6f-193">布尔值</span><span class="sxs-lookup"><span data-stu-id="f4c6f-193">Boolean</span></span> | <span data-ttu-id="f4c6f-194">如果会议组织者允许被邀请者在响应时建议新时间，则为`True`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-194">`True` if the meeting organizer allows invitees to propose a new time when responding, `false` otherwise.</span></span> <span data-ttu-id="f4c6f-195">可选。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-195">Optional.</span></span> <span data-ttu-id="f4c6f-196">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-196">Default is `true`.</span></span> |
|<span data-ttu-id="f4c6f-197">attendees</span><span class="sxs-lookup"><span data-stu-id="f4c6f-197">attendees</span></span>|<span data-ttu-id="f4c6f-198">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-198">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="f4c6f-199">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-199">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="f4c6f-200">body</span><span class="sxs-lookup"><span data-stu-id="f4c6f-200">body</span></span>|[<span data-ttu-id="f4c6f-201">itemBody</span><span class="sxs-lookup"><span data-stu-id="f4c6f-201">itemBody</span></span>](itembody.md)|<span data-ttu-id="f4c6f-p107">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p107">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="f4c6f-204">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="f4c6f-204">bodyPreview</span></span>|<span data-ttu-id="f4c6f-205">字符串</span><span class="sxs-lookup"><span data-stu-id="f4c6f-205">String</span></span>|<span data-ttu-id="f4c6f-p108">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p108">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="f4c6f-208">categories</span><span class="sxs-lookup"><span data-stu-id="f4c6f-208">categories</span></span>|<span data-ttu-id="f4c6f-209">String collection</span><span class="sxs-lookup"><span data-stu-id="f4c6f-209">String collection</span></span>|<span data-ttu-id="f4c6f-210">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-210">The categories associated with the event.</span></span>|
|<span data-ttu-id="f4c6f-211">changeKey</span><span class="sxs-lookup"><span data-stu-id="f4c6f-211">changeKey</span></span>|<span data-ttu-id="f4c6f-212">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-212">String</span></span>|<span data-ttu-id="f4c6f-p109">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p109">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="f4c6f-216">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4c6f-216">createdDateTime</span></span>|<span data-ttu-id="f4c6f-217">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4c6f-217">DateTimeOffset</span></span>|<span data-ttu-id="f4c6f-p110">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p110">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4c6f-220">end</span><span class="sxs-lookup"><span data-stu-id="f4c6f-220">end</span></span>|[<span data-ttu-id="f4c6f-221">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4c6f-221">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f4c6f-222">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-222">The date, time, and time zone that the event ends.</span></span> <span data-ttu-id="f4c6f-223">默认情况下，结束时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-223">By default, the end time is in UTC.</span></span>|
|<span data-ttu-id="f4c6f-224">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="f4c6f-224">hasAttachments</span></span>|<span data-ttu-id="f4c6f-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-225">Boolean</span></span>|<span data-ttu-id="f4c6f-226">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-226">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="f4c6f-227">iCalUId</span><span class="sxs-lookup"><span data-stu-id="f4c6f-227">iCalUId</span></span>|<span data-ttu-id="f4c6f-228">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-228">String</span></span>|<span data-ttu-id="f4c6f-229">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-229">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="f4c6f-230">只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-230">Read-only.</span></span>|
|<span data-ttu-id="f4c6f-231">id</span><span class="sxs-lookup"><span data-stu-id="f4c6f-231">id</span></span>|<span data-ttu-id="f4c6f-232">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-232">String</span></span>| <span data-ttu-id="f4c6f-233">只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-233">Read-only.</span></span>|
|<span data-ttu-id="f4c6f-234">importance</span><span class="sxs-lookup"><span data-stu-id="f4c6f-234">importance</span></span>|<span data-ttu-id="f4c6f-235">importance</span><span class="sxs-lookup"><span data-stu-id="f4c6f-235">importance</span></span>|<span data-ttu-id="f4c6f-236">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-236">The importance of the event.</span></span> <span data-ttu-id="f4c6f-237">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-237">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="f4c6f-238">isAllDay</span><span class="sxs-lookup"><span data-stu-id="f4c6f-238">isAllDay</span></span>|<span data-ttu-id="f4c6f-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-239">Boolean</span></span>|<span data-ttu-id="f4c6f-240">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-240">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="f4c6f-241">isCancelled</span><span class="sxs-lookup"><span data-stu-id="f4c6f-241">isCancelled</span></span>|<span data-ttu-id="f4c6f-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-242">Boolean</span></span>|<span data-ttu-id="f4c6f-243">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-243">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="f4c6f-244">isOnlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f4c6f-244">isOnlineMeeting</span></span>|<span data-ttu-id="f4c6f-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-245">Boolean</span></span>| <span data-ttu-id="f4c6f-246">若此事件包含联机会议信息则为 `True`，反之则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-246">`True` if this event has online meeting information, `false` otherwise.</span></span> <span data-ttu-id="f4c6f-247">默认为 false。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-247">Default is false.</span></span> <span data-ttu-id="f4c6f-248">可选。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-248">Optional.</span></span>|
|<span data-ttu-id="f4c6f-249">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="f4c6f-249">isOrganizer</span></span>|<span data-ttu-id="f4c6f-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-250">Boolean</span></span>|<span data-ttu-id="f4c6f-251">如果日历所有者（通过“[日历](calendar.md)”的“**所有者**”属性指定）是事件的组织者（通过“**事件**”的“**组织者**”属性指定），设定为 true。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-251">Set to true if the calendar owner (specified by the **owner** property of the [calendar](calendar.md)) is the organizer of the event (specified by the **organizer** property of the **event**).</span></span> <span data-ttu-id="f4c6f-252">这也适用于代理人代表所有者组织事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-252">This also applies if a delegate organized the event on behalf of the owner.</span></span>|
|<span data-ttu-id="f4c6f-253">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="f4c6f-253">isReminderOn</span></span>|<span data-ttu-id="f4c6f-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="f4c6f-254">Boolean</span></span>|<span data-ttu-id="f4c6f-255">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-255">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="f4c6f-256">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4c6f-256">lastModifiedDateTime</span></span>|<span data-ttu-id="f4c6f-257">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4c6f-257">DateTimeOffset</span></span>|<span data-ttu-id="f4c6f-p116">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p116">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4c6f-260">location</span><span class="sxs-lookup"><span data-stu-id="f4c6f-260">location</span></span>|[<span data-ttu-id="f4c6f-261">位置</span><span class="sxs-lookup"><span data-stu-id="f4c6f-261">location</span></span>](location.md)|<span data-ttu-id="f4c6f-262">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-262">The location of the event.</span></span>|
|<span data-ttu-id="f4c6f-263">locations</span><span class="sxs-lookup"><span data-stu-id="f4c6f-263">locations</span></span>|<span data-ttu-id="f4c6f-264">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-264">[location](location.md) collection</span></span>|<span data-ttu-id="f4c6f-265">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-265">The locations where the event is held or attended from.</span></span> <span data-ttu-id="f4c6f-266">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-266">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="f4c6f-267">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-267">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="f4c6f-268">onlineMeeting</span><span class="sxs-lookup"><span data-stu-id="f4c6f-268">onlineMeeting</span></span>|[<span data-ttu-id="f4c6f-269">OnlineMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="f4c6f-269">OnlineMeetingInfo</span></span>](onlinemeetinginfo.md)| <span data-ttu-id="f4c6f-270">关于与会者如何加入联机会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-270">Details for an attendee to join the meeting online.</span></span> <span data-ttu-id="f4c6f-271">只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-271">Read-only.</span></span>|
|<span data-ttu-id="f4c6f-272">onlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="f4c6f-272">onlineMeetingProvider</span></span>|<span data-ttu-id="f4c6f-273">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="f4c6f-273">onlineMeetingProviderType</span></span>| <span data-ttu-id="f4c6f-274">表示联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-274">Represents the online meeting service provider.</span></span> <span data-ttu-id="f4c6f-275">可取值为：`teamsForBusiness`、`skypeForBusiness` 和 `skypeForConsumer`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-275">The possible values are `teamsForBusiness`, `skypeForBusiness`, and `skypeForConsumer`.</span></span> <span data-ttu-id="f4c6f-276">可选。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-276">Optional.</span></span> |
|<span data-ttu-id="f4c6f-277">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="f4c6f-277">onlineMeetingUrl</span></span>|<span data-ttu-id="f4c6f-278">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-278">String</span></span>|<span data-ttu-id="f4c6f-279">联机会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-279">A URL for an online meeting.</span></span> <span data-ttu-id="f4c6f-280">仅当组织者将事件指定为联机会议（如 Skype 会议）时才会设置此属性。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-280">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="f4c6f-281">只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-281">Read-only.</span></span>|
|<span data-ttu-id="f4c6f-282">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="f4c6f-282">organizer</span></span>|[<span data-ttu-id="f4c6f-283">recipient</span><span class="sxs-lookup"><span data-stu-id="f4c6f-283">recipient</span></span>](recipient.md)|<span data-ttu-id="f4c6f-284">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-284">The organizer of the event.</span></span>|
|<span data-ttu-id="f4c6f-285">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4c6f-285">originalEndTimeZone</span></span>|<span data-ttu-id="f4c6f-286">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-286">String</span></span>|<span data-ttu-id="f4c6f-287">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-287">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="f4c6f-288">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-288">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="f4c6f-289">originalStart</span><span class="sxs-lookup"><span data-stu-id="f4c6f-289">originalStart</span></span>|<span data-ttu-id="f4c6f-290">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4c6f-290">DateTimeOffset</span></span>|<span data-ttu-id="f4c6f-p122">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4c6f-293">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4c6f-293">originalStartTimeZone</span></span>|<span data-ttu-id="f4c6f-294">字符串</span><span class="sxs-lookup"><span data-stu-id="f4c6f-294">String</span></span>|<span data-ttu-id="f4c6f-p123">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p123">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="f4c6f-297">recurrence</span><span class="sxs-lookup"><span data-stu-id="f4c6f-297">recurrence</span></span>|[<span data-ttu-id="f4c6f-298">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="f4c6f-298">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="f4c6f-299">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-299">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="f4c6f-300">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="f4c6f-300">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="f4c6f-301">Int32</span><span class="sxs-lookup"><span data-stu-id="f4c6f-301">Int32</span></span>|<span data-ttu-id="f4c6f-302">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-302">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="f4c6f-303">responseRequested</span><span class="sxs-lookup"><span data-stu-id="f4c6f-303">responseRequested</span></span>|<span data-ttu-id="f4c6f-304">布尔值</span><span class="sxs-lookup"><span data-stu-id="f4c6f-304">Boolean</span></span>|<span data-ttu-id="f4c6f-305">默认值为 true，表示组织者愿意被邀请者发送事件响应。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-305">Default is true, which represents the organizer would like an invitee to send a response to the event.</span></span>|
|<span data-ttu-id="f4c6f-306">responseStatus</span><span class="sxs-lookup"><span data-stu-id="f4c6f-306">responseStatus</span></span>|[<span data-ttu-id="f4c6f-307">responseStatus</span><span class="sxs-lookup"><span data-stu-id="f4c6f-307">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="f4c6f-308">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-308">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="f4c6f-309">sensitivity</span><span class="sxs-lookup"><span data-stu-id="f4c6f-309">sensitivity</span></span>|<span data-ttu-id="f4c6f-310">敏感度</span><span class="sxs-lookup"><span data-stu-id="f4c6f-310">sensitivity</span></span>| <span data-ttu-id="f4c6f-311">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-311">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="f4c6f-312">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="f4c6f-312">seriesMasterId</span></span>|<span data-ttu-id="f4c6f-313">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-313">String</span></span>|<span data-ttu-id="f4c6f-314">定期系列主项的 ID（如果此事件是定期系列的一部分）。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-314">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="f4c6f-315">showAs</span><span class="sxs-lookup"><span data-stu-id="f4c6f-315">showAs</span></span>|<span data-ttu-id="f4c6f-316">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="f4c6f-316">freeBusyStatus</span></span>|<span data-ttu-id="f4c6f-317">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-317">The status to show.</span></span> <span data-ttu-id="f4c6f-318">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-318">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="f4c6f-319">start</span><span class="sxs-lookup"><span data-stu-id="f4c6f-319">start</span></span>|[<span data-ttu-id="f4c6f-320">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="f4c6f-320">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="f4c6f-321">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-321">The date, time, and time zone that the event starts.</span></span> <span data-ttu-id="f4c6f-322">默认情况下，开始时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-322">By default, the start time is in UTC.</span></span>|
|<span data-ttu-id="f4c6f-323">subject</span><span class="sxs-lookup"><span data-stu-id="f4c6f-323">subject</span></span>|<span data-ttu-id="f4c6f-324">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-324">String</span></span>|<span data-ttu-id="f4c6f-325">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-325">The text of the event's subject line.</span></span>|
|<span data-ttu-id="f4c6f-326">type</span><span class="sxs-lookup"><span data-stu-id="f4c6f-326">type</span></span>|<span data-ttu-id="f4c6f-327">eventType</span><span class="sxs-lookup"><span data-stu-id="f4c6f-327">eventType</span></span>|<span data-ttu-id="f4c6f-328">事件类型。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-328">The event type.</span></span> <span data-ttu-id="f4c6f-329">可能的值包括 `singleInstance`、`occurrence`、`exception`、`seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-329">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="f4c6f-330">只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-330">Read-only.</span></span>|
|<span data-ttu-id="f4c6f-331">webLink</span><span class="sxs-lookup"><span data-stu-id="f4c6f-331">webLink</span></span>|<span data-ttu-id="f4c6f-332">String</span><span class="sxs-lookup"><span data-stu-id="f4c6f-332">String</span></span>|<span data-ttu-id="f4c6f-333">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-333">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="f4c6f-334">如果登录邮件，则 Outlook 网页面会在浏览器中打开事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-334">Outlook on the web opens the event in the browser if you are signed in to your mailbox.</span></span> <span data-ttu-id="f4c6f-335">否则，Outlook 网页面会提示你进行登录。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-335">Otherwise, Outlook on the web prompts you to sign in.</span></span><br/><br/><span data-ttu-id="f4c6f-336">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-336">This URL can be accessed from within an iFrame.</span></span>|

> [!NOTE]
> <span data-ttu-id="f4c6f-337">**webLink** 属性指定了一个 URL，它仅在 Outlook 网页版早期版本中打开事件。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-337">The **webLink** property specifies a URL that opens the event in only earlier versions of Outlook on the web.</span></span> <span data-ttu-id="f4c6f-338">以下是 URL 格式，其中 _{event-id}_ 是 **id** 属性的 _**URL 编码**_ 值：</span><span class="sxs-lookup"><span data-stu-id="f4c6f-338">The following are the URL formats, with _{event-id}_ being the _**URL-encoded**_ value of the **id** property:</span></span>
>
> * <span data-ttu-id="f4c6f-339">对于工作或学校帐户：`https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-339">For work or school accounts: `https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> * <span data-ttu-id="f4c6f-340">对于 Microsoft 帐户：`https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-340">For Microsoft accounts: `https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> <span data-ttu-id="f4c6f-341">要在 Outlook 网页版的当前版本中打开事件，请将 URL 转换为下述格式之一，并使用该 URL 打开事件：</span><span class="sxs-lookup"><span data-stu-id="f4c6f-341">To open the event in a current version of Outlook on the web, convert the URL to one of the following formats, and use that URL to open the event:</span></span>
>
> * <span data-ttu-id="f4c6f-342">对于工作或学校帐户：`https://outlook.office365.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-342">For work or school accounts: `https://outlook.office365.com/calendar/item/{event-id}`</span></span>
>
> * <span data-ttu-id="f4c6f-343">对于 Microsoft 帐户：`https://outlook.live.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="f4c6f-343">For Microsoft accounts: `https://outlook.live.com/calendar/item/{event-id}`</span></span>


## <a name="relationships"></a><span data-ttu-id="f4c6f-344">关系</span><span class="sxs-lookup"><span data-stu-id="f4c6f-344">Relationships</span></span>
| <span data-ttu-id="f4c6f-345">关系</span><span class="sxs-lookup"><span data-stu-id="f4c6f-345">Relationship</span></span> | <span data-ttu-id="f4c6f-346">类型</span><span class="sxs-lookup"><span data-stu-id="f4c6f-346">Type</span></span>   |<span data-ttu-id="f4c6f-347">说明</span><span class="sxs-lookup"><span data-stu-id="f4c6f-347">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c6f-348">attachments</span><span class="sxs-lookup"><span data-stu-id="f4c6f-348">attachments</span></span>|<span data-ttu-id="f4c6f-349">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-349">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="f4c6f-p129">事件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p129">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f4c6f-354">日历</span><span class="sxs-lookup"><span data-stu-id="f4c6f-354">calendar</span></span>|[<span data-ttu-id="f4c6f-355">日历</span><span class="sxs-lookup"><span data-stu-id="f4c6f-355">calendar</span></span>](calendar.md)|<span data-ttu-id="f4c6f-p130">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p130">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="f4c6f-359">extensions</span><span class="sxs-lookup"><span data-stu-id="f4c6f-359">extensions</span></span>|<span data-ttu-id="f4c6f-360">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-360">[Extension](extension.md) collection</span></span>|<span data-ttu-id="f4c6f-p131">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p131">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f4c6f-364">instances</span><span class="sxs-lookup"><span data-stu-id="f4c6f-364">instances</span></span>|<span data-ttu-id="f4c6f-365">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-365">[event](event.md) collection</span></span>|<span data-ttu-id="f4c6f-p132">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p132">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f4c6f-370">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f4c6f-370">multiValueExtendedProperties</span></span>|<span data-ttu-id="f4c6f-371">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f4c6f-371">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f4c6f-p133">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p133">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="f4c6f-375">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="f4c6f-375">singleValueExtendedProperties</span></span>|<span data-ttu-id="f4c6f-376">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="f4c6f-376">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="f4c6f-p134">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-p134">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4c6f-380">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f4c6f-380">JSON representation</span></span>

<span data-ttu-id="f4c6f-381">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f4c6f-381">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="f4c6f-382">另请参阅</span><span class="sxs-lookup"><span data-stu-id="f4c6f-382">See also</span></span>

- [<span data-ttu-id="f4c6f-383">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="f4c6f-383">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="f4c6f-384">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="f4c6f-384">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="f4c6f-385">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f4c6f-385">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="f4c6f-386">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f4c6f-386">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="f4c6f-387">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="f4c6f-387">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
