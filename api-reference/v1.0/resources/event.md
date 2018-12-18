---
title: 事件资源类型
description: 日历中的事件。
author: angelgolfer-ms
ms.openlocfilehash: 2caa1cb51da5f9d9ae8808b574e2787fbb63da46
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356593"
---
# <a name="event-resource-type"></a><span data-ttu-id="3f308-103">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="3f308-103">event resource type</span></span>

<span data-ttu-id="3f308-104">日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-104">An event in a calendar.</span></span>

<span data-ttu-id="3f308-105">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="3f308-105">This resource supports:</span></span>

- <span data-ttu-id="3f308-106">将您自己的数据添加到自定义属性，作为[扩展](/graph/extensibility-overview)。</span><span class="sxs-lookup"><span data-stu-id="3f308-106">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="3f308-107">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="3f308-107">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="3f308-108">通过提供 [delta](../api/event-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="3f308-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="3f308-109">方法</span><span class="sxs-lookup"><span data-stu-id="3f308-109">Methods</span></span>

| <span data-ttu-id="3f308-110">方法</span><span class="sxs-lookup"><span data-stu-id="3f308-110">Method</span></span>       | <span data-ttu-id="3f308-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="3f308-111">Return Type</span></span>  |<span data-ttu-id="3f308-112">说明</span><span class="sxs-lookup"><span data-stu-id="3f308-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3f308-113">列出事件</span><span class="sxs-lookup"><span data-stu-id="3f308-113">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="3f308-114">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-114">[event](event.md) collection</span></span> |<span data-ttu-id="3f308-p101">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="3f308-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="3f308-117">创建事件</span><span class="sxs-lookup"><span data-stu-id="3f308-117">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="3f308-118">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-118">event</span></span>](event.md)| <span data-ttu-id="3f308-119">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-119">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="3f308-120">获取事件</span><span class="sxs-lookup"><span data-stu-id="3f308-120">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="3f308-121">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-121">event</span></span>](event.md) |<span data-ttu-id="3f308-122">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3f308-122">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="3f308-123">更新</span><span class="sxs-lookup"><span data-stu-id="3f308-123">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="3f308-124">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-124">event</span></span>](event.md) |<span data-ttu-id="3f308-125">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="3f308-125">Update event object.</span></span> |
|[<span data-ttu-id="3f308-126">删除</span><span class="sxs-lookup"><span data-stu-id="3f308-126">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="3f308-127">无</span><span class="sxs-lookup"><span data-stu-id="3f308-127">None</span></span> |<span data-ttu-id="3f308-128">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="3f308-128">Delete event object.</span></span> |
|[<span data-ttu-id="3f308-129">接受</span><span class="sxs-lookup"><span data-stu-id="3f308-129">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="3f308-130">无</span><span class="sxs-lookup"><span data-stu-id="3f308-130">None</span></span>|<span data-ttu-id="3f308-131">接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-131">Accept the specified event.</span></span>|
|[<span data-ttu-id="3f308-132">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="3f308-132">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="3f308-133">无</span><span class="sxs-lookup"><span data-stu-id="3f308-133">None</span></span>|<span data-ttu-id="3f308-134">暂时接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-134">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="3f308-135">拒绝</span><span class="sxs-lookup"><span data-stu-id="3f308-135">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="3f308-136">无</span><span class="sxs-lookup"><span data-stu-id="3f308-136">None</span></span>|<span data-ttu-id="3f308-137">拒绝对指定事件的邀请。</span><span class="sxs-lookup"><span data-stu-id="3f308-137">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="3f308-138">delta</span><span class="sxs-lookup"><span data-stu-id="3f308-138">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="3f308-139">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f308-139">[event](event.md) collection</span></span>|<span data-ttu-id="3f308-140">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="3f308-140">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="3f308-141">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="3f308-141">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="3f308-142">无</span><span class="sxs-lookup"><span data-stu-id="3f308-142">None</span></span>|<span data-ttu-id="3f308-143">消除指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="3f308-143">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="3f308-144">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="3f308-144">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="3f308-145">无</span><span class="sxs-lookup"><span data-stu-id="3f308-145">None</span></span>|<span data-ttu-id="3f308-146">暂停指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="3f308-146">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="3f308-147">列出实例</span><span class="sxs-lookup"><span data-stu-id="3f308-147">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="3f308-148">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-148">[event](event.md) collection</span></span>| <span data-ttu-id="3f308-p102">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="3f308-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="3f308-151">**附件**</span><span class="sxs-lookup"><span data-stu-id="3f308-151">**Attachments**</span></span>| | |
|[<span data-ttu-id="3f308-152">列出附件</span><span class="sxs-lookup"><span data-stu-id="3f308-152">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="3f308-153">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-153">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="3f308-154">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="3f308-154">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="3f308-155">Add attachment</span><span class="sxs-lookup"><span data-stu-id="3f308-155">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="3f308-156">attachment</span><span class="sxs-lookup"><span data-stu-id="3f308-156">attachment</span></span>](attachment.md)| <span data-ttu-id="3f308-157">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="3f308-157">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="3f308-158">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="3f308-158">**Open extensions**</span></span>| | |
|[<span data-ttu-id="3f308-159">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="3f308-159">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="3f308-160">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="3f308-160">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="3f308-161">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3f308-161">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="3f308-162">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="3f308-162">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="3f308-163">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-163">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="3f308-164">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="3f308-164">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="3f308-165">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="3f308-165">**Extended properties**</span></span>| | |
|[<span data-ttu-id="3f308-166">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="3f308-166">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="3f308-167">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-167">event</span></span>](event.md)  |<span data-ttu-id="3f308-168">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3f308-168">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="3f308-169">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="3f308-169">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3f308-170">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-170">event</span></span>](event.md) | <span data-ttu-id="3f308-171">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-171">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="3f308-172">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="3f308-172">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="3f308-173">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-173">event</span></span>](event.md) | <span data-ttu-id="3f308-174">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3f308-174">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="3f308-175">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="3f308-175">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3f308-176">事件</span><span class="sxs-lookup"><span data-stu-id="3f308-176">event</span></span>](event.md) | <span data-ttu-id="3f308-177">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="3f308-177">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="3f308-178">属性</span><span class="sxs-lookup"><span data-stu-id="3f308-178">Properties</span></span>
| <span data-ttu-id="3f308-179">属性</span><span class="sxs-lookup"><span data-stu-id="3f308-179">Property</span></span>     | <span data-ttu-id="3f308-180">类型</span><span class="sxs-lookup"><span data-stu-id="3f308-180">Type</span></span>   |<span data-ttu-id="3f308-181">说明</span><span class="sxs-lookup"><span data-stu-id="3f308-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f308-182">attendees</span><span class="sxs-lookup"><span data-stu-id="3f308-182">attendees</span></span>|<span data-ttu-id="3f308-183">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-183">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="3f308-184">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="3f308-184">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="3f308-185">body</span><span class="sxs-lookup"><span data-stu-id="3f308-185">body</span></span>|[<span data-ttu-id="3f308-186">itemBody</span><span class="sxs-lookup"><span data-stu-id="3f308-186">itemBody</span></span>](itembody.md)|<span data-ttu-id="3f308-p103">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="3f308-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="3f308-189">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="3f308-189">bodyPreview</span></span>|<span data-ttu-id="3f308-190">字符串</span><span class="sxs-lookup"><span data-stu-id="3f308-190">String</span></span>|<span data-ttu-id="3f308-p104">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="3f308-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="3f308-193">categories</span><span class="sxs-lookup"><span data-stu-id="3f308-193">categories</span></span>|<span data-ttu-id="3f308-194">String collection</span><span class="sxs-lookup"><span data-stu-id="3f308-194">String collection</span></span>|<span data-ttu-id="3f308-195">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="3f308-195">The categories associated with the event.</span></span>|
|<span data-ttu-id="3f308-196">changeKey</span><span class="sxs-lookup"><span data-stu-id="3f308-196">changeKey</span></span>|<span data-ttu-id="3f308-197">String</span><span class="sxs-lookup"><span data-stu-id="3f308-197">String</span></span>|<span data-ttu-id="3f308-p105">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="3f308-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3f308-201">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f308-201">createdDateTime</span></span>|<span data-ttu-id="3f308-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f308-202">DateTimeOffset</span></span>|<span data-ttu-id="3f308-p106">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3f308-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3f308-205">end</span><span class="sxs-lookup"><span data-stu-id="3f308-205">end</span></span>|[<span data-ttu-id="3f308-206">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3f308-206">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3f308-207">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3f308-207">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="3f308-208">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="3f308-208">hasAttachments</span></span>|<span data-ttu-id="3f308-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-209">Boolean</span></span>|<span data-ttu-id="3f308-210">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-210">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="3f308-211">iCalUId</span><span class="sxs-lookup"><span data-stu-id="3f308-211">iCalUId</span></span>|<span data-ttu-id="3f308-212">String</span><span class="sxs-lookup"><span data-stu-id="3f308-212">String</span></span>|<span data-ttu-id="3f308-213">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f308-213">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="3f308-214">只读。</span><span class="sxs-lookup"><span data-stu-id="3f308-214">Read-only.</span></span>|
|<span data-ttu-id="3f308-215">id</span><span class="sxs-lookup"><span data-stu-id="3f308-215">id</span></span>|<span data-ttu-id="3f308-216">String</span><span class="sxs-lookup"><span data-stu-id="3f308-216">String</span></span>| <span data-ttu-id="3f308-217">只读。</span><span class="sxs-lookup"><span data-stu-id="3f308-217">Read-only.</span></span>|
|<span data-ttu-id="3f308-218">importance</span><span class="sxs-lookup"><span data-stu-id="3f308-218">importance</span></span>|<span data-ttu-id="3f308-219">importance</span><span class="sxs-lookup"><span data-stu-id="3f308-219">importance</span></span>|<span data-ttu-id="3f308-220">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="3f308-220">The importance of the event.</span></span> <span data-ttu-id="3f308-221">可能的值为： `low`， `normal`， `high`。</span><span class="sxs-lookup"><span data-stu-id="3f308-221">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="3f308-222">isAllDay</span><span class="sxs-lookup"><span data-stu-id="3f308-222">isAllDay</span></span>|<span data-ttu-id="3f308-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-223">Boolean</span></span>|<span data-ttu-id="3f308-224">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-224">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="3f308-225">isCancelled</span><span class="sxs-lookup"><span data-stu-id="3f308-225">isCancelled</span></span>|<span data-ttu-id="3f308-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-226">Boolean</span></span>|<span data-ttu-id="3f308-227">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-227">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="3f308-228">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="3f308-228">isOrganizer</span></span>|<span data-ttu-id="3f308-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-229">Boolean</span></span>|<span data-ttu-id="3f308-230">如果邮件发件人也是组织者，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-230">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="3f308-231">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="3f308-231">isReminderOn</span></span>|<span data-ttu-id="3f308-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-232">Boolean</span></span>|<span data-ttu-id="3f308-233">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-233">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="3f308-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f308-234">lastModifiedDateTime</span></span>|<span data-ttu-id="3f308-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f308-235">DateTimeOffset</span></span>|<span data-ttu-id="3f308-p109">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3f308-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3f308-238">location</span><span class="sxs-lookup"><span data-stu-id="3f308-238">location</span></span>|[<span data-ttu-id="3f308-239">位置</span><span class="sxs-lookup"><span data-stu-id="3f308-239">location</span></span>](location.md)|<span data-ttu-id="3f308-240">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="3f308-240">The location of the event.</span></span>|
|<span data-ttu-id="3f308-241">locations</span><span class="sxs-lookup"><span data-stu-id="3f308-241">locations</span></span>|<span data-ttu-id="3f308-242">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-242">[location](location.md) collection</span></span>|<span data-ttu-id="3f308-243">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="3f308-243">The locations where the event is held or attended from.</span></span> <span data-ttu-id="3f308-244">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="3f308-244">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="3f308-245">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="3f308-245">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="3f308-246">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="3f308-246">onlineMeetingUrl</span></span>|<span data-ttu-id="3f308-247">String</span><span class="sxs-lookup"><span data-stu-id="3f308-247">String</span></span>|<span data-ttu-id="3f308-248">在线会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="3f308-248">A URL for an online meeting.</span></span> <span data-ttu-id="3f308-249">仅组织者指定为联机会议如 Skype 会议事件时，该属性是设置。</span><span class="sxs-lookup"><span data-stu-id="3f308-249">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="3f308-250">只读。</span><span class="sxs-lookup"><span data-stu-id="3f308-250">Read-only.</span></span>|
|<span data-ttu-id="3f308-251">organizer</span><span class="sxs-lookup"><span data-stu-id="3f308-251">organizer</span></span>|[<span data-ttu-id="3f308-252">recipient</span><span class="sxs-lookup"><span data-stu-id="3f308-252">recipient</span></span>](recipient.md)|<span data-ttu-id="3f308-253">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="3f308-253">The organizer of the event.</span></span>|
|<span data-ttu-id="3f308-254">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="3f308-254">originalEndTimeZone</span></span>|<span data-ttu-id="3f308-255">String</span><span class="sxs-lookup"><span data-stu-id="3f308-255">String</span></span>|<span data-ttu-id="3f308-256">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="3f308-256">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="3f308-257">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="3f308-257">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="3f308-258">originalStart</span><span class="sxs-lookup"><span data-stu-id="3f308-258">originalStart</span></span>|<span data-ttu-id="3f308-259">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f308-259">DateTimeOffset</span></span>|<span data-ttu-id="3f308-p113">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3f308-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3f308-262">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="3f308-262">originalStartTimeZone</span></span>|<span data-ttu-id="3f308-263">字符串</span><span class="sxs-lookup"><span data-stu-id="3f308-263">String</span></span>|<span data-ttu-id="3f308-p114">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="3f308-p114">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="3f308-266">recurrence</span><span class="sxs-lookup"><span data-stu-id="3f308-266">recurrence</span></span>|[<span data-ttu-id="3f308-267">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="3f308-267">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="3f308-268">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="3f308-268">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="3f308-269">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="3f308-269">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="3f308-270">Int32</span><span class="sxs-lookup"><span data-stu-id="3f308-270">Int32</span></span>|<span data-ttu-id="3f308-271">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3f308-271">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="3f308-272">responseRequested</span><span class="sxs-lookup"><span data-stu-id="3f308-272">responseRequested</span></span>|<span data-ttu-id="3f308-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="3f308-273">Boolean</span></span>|<span data-ttu-id="3f308-274">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3f308-274">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="3f308-275">responseStatus</span><span class="sxs-lookup"><span data-stu-id="3f308-275">responseStatus</span></span>|[<span data-ttu-id="3f308-276">responseStatus</span><span class="sxs-lookup"><span data-stu-id="3f308-276">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="3f308-277">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="3f308-277">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="3f308-278">sensitivity</span><span class="sxs-lookup"><span data-stu-id="3f308-278">sensitivity</span></span>|<span data-ttu-id="3f308-279">sensitivity</span><span class="sxs-lookup"><span data-stu-id="3f308-279">sensitivity</span></span>| <span data-ttu-id="3f308-280">可能的值为： `normal`， `personal`， `private`， `confidential`。</span><span class="sxs-lookup"><span data-stu-id="3f308-280">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="3f308-281">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="3f308-281">seriesMasterId</span></span>|<span data-ttu-id="3f308-282">String</span><span class="sxs-lookup"><span data-stu-id="3f308-282">String</span></span>|<span data-ttu-id="3f308-283">定期系列主项目，如果该事件是定期系列的一部分的 ID。</span><span class="sxs-lookup"><span data-stu-id="3f308-283">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="3f308-284">showAs</span><span class="sxs-lookup"><span data-stu-id="3f308-284">showAs</span></span>|<span data-ttu-id="3f308-285">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="3f308-285">freeBusyStatus</span></span>|<span data-ttu-id="3f308-286">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="3f308-286">The status to show.</span></span> <span data-ttu-id="3f308-287">可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="3f308-287">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="3f308-288">start</span><span class="sxs-lookup"><span data-stu-id="3f308-288">start</span></span>|[<span data-ttu-id="3f308-289">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3f308-289">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3f308-290">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3f308-290">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3f308-291">subject</span><span class="sxs-lookup"><span data-stu-id="3f308-291">subject</span></span>|<span data-ttu-id="3f308-292">String</span><span class="sxs-lookup"><span data-stu-id="3f308-292">String</span></span>|<span data-ttu-id="3f308-293">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="3f308-293">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3f308-294">type</span><span class="sxs-lookup"><span data-stu-id="3f308-294">type</span></span>|<span data-ttu-id="3f308-295">eventType</span><span class="sxs-lookup"><span data-stu-id="3f308-295">eventType</span></span>|<span data-ttu-id="3f308-296">事件类型。</span><span class="sxs-lookup"><span data-stu-id="3f308-296">The event type.</span></span> <span data-ttu-id="3f308-297">可能的值为： `singleInstance`， `occurrence`， `exception`， `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="3f308-297">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="3f308-298">只读。</span><span class="sxs-lookup"><span data-stu-id="3f308-298">Read-only.</span></span>|
|<span data-ttu-id="3f308-299">webLink</span><span class="sxs-lookup"><span data-stu-id="3f308-299">webLink</span></span>|<span data-ttu-id="3f308-300">String</span><span class="sxs-lookup"><span data-stu-id="3f308-300">String</span></span>|<span data-ttu-id="3f308-301">要在 Outlook Web App 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="3f308-301">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="3f308-p117">如果你通过 Outlook Web App 登录邮箱，该事件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="3f308-p117">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3f308-304">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="3f308-304">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f308-305">关系</span><span class="sxs-lookup"><span data-stu-id="3f308-305">Relationships</span></span>
| <span data-ttu-id="3f308-306">关系</span><span class="sxs-lookup"><span data-stu-id="3f308-306">Relationship</span></span> | <span data-ttu-id="3f308-307">类型</span><span class="sxs-lookup"><span data-stu-id="3f308-307">Type</span></span>   |<span data-ttu-id="3f308-308">说明</span><span class="sxs-lookup"><span data-stu-id="3f308-308">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f308-309">attachments</span><span class="sxs-lookup"><span data-stu-id="3f308-309">attachments</span></span>|<span data-ttu-id="3f308-310">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-310">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="3f308-p118">事件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f308-p118">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3f308-315">日历</span><span class="sxs-lookup"><span data-stu-id="3f308-315">calendar</span></span>|[<span data-ttu-id="3f308-316">日历</span><span class="sxs-lookup"><span data-stu-id="3f308-316">calendar</span></span>](calendar.md)|<span data-ttu-id="3f308-p119">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="3f308-p119">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="3f308-320">extensions</span><span class="sxs-lookup"><span data-stu-id="3f308-320">extensions</span></span>|<span data-ttu-id="3f308-321">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="3f308-321">[Extension](extension.md) collection</span></span>|<span data-ttu-id="3f308-p120">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f308-p120">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3f308-325">instances</span><span class="sxs-lookup"><span data-stu-id="3f308-325">instances</span></span>|<span data-ttu-id="3f308-326">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-326">[event](event.md) collection</span></span>|<span data-ttu-id="3f308-p121">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f308-p121">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3f308-331">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3f308-331">multiValueExtendedProperties</span></span>|<span data-ttu-id="3f308-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3f308-332">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3f308-p122">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f308-p122">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3f308-336">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3f308-336">singleValueExtendedProperties</span></span>|<span data-ttu-id="3f308-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="3f308-337">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3f308-p123">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3f308-p123">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3f308-341">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f308-341">JSON representation</span></span>

<span data-ttu-id="3f308-342">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f308-342">Here is a JSON representation of the resource</span></span>

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
  "isOrganizer": true,
  "isReminderOn": true,
  "lastModifiedDateTime": "String (timestamp)",
  "location": {"@odata.type": "microsoft.graph.location"},
  "locations": [{"@odata.type": "microsoft.graph.location"}],
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


## <a name="see-also"></a><span data-ttu-id="3f308-343">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3f308-343">See also</span></span>

- [<span data-ttu-id="3f308-344">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="3f308-344">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="3f308-345">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="3f308-345">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="3f308-346">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3f308-346">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3f308-347">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3f308-347">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3f308-348">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3f308-348">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
