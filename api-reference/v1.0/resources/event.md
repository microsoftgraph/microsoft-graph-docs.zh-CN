---
title: 事件资源类型
description: 日历中的事件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 0be46df98faf4540e221a140daf0ec22355fc24a
ms.sourcegitcommit: 9cee9d8229fc84dd7ef97670ff27c145e1a78408
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2019
ms.locfileid: "35778724"
---
# <a name="event-resource-type"></a><span data-ttu-id="3e212-103">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="3e212-103">event resource type</span></span>

<span data-ttu-id="3e212-104">[用户](user.md)日历或 Office 365 [组](group.md)日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-104">An event in a [user](user.md) calendar, or the default calendar of an Office 365 [group](group.md).</span></span>

<span data-ttu-id="3e212-105">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="3e212-105">This resource supports:</span></span>

- <span data-ttu-id="3e212-106">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3e212-106">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="3e212-107">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="3e212-107">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="3e212-108">通过提供 [delta](../api/event-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="3e212-108">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>

> <span data-ttu-id="3e212-109">**注释：** 与用户日历、组日历及其事件交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="3e212-109">**Note:** There are a few minor differences in the way you can interact with user calendars, group calendars, and their events:</span></span>

- <span data-ttu-id="3e212-110">只可以组织 [calendarGroup](calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="3e212-110">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="3e212-111">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="3e212-111">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="3e212-112">只可以[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)_用户_日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="3e212-112">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for _user_ calendars only.</span></span>
- <span data-ttu-id="3e212-113">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="3e212-113">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="3e212-114">只可以[暂停](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)_用户_日历中的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="3e212-114">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for _user_ calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="3e212-115">方法</span><span class="sxs-lookup"><span data-stu-id="3e212-115">Methods</span></span>

| <span data-ttu-id="3e212-116">方法</span><span class="sxs-lookup"><span data-stu-id="3e212-116">Method</span></span>       | <span data-ttu-id="3e212-117">返回类型</span><span class="sxs-lookup"><span data-stu-id="3e212-117">Return Type</span></span>  |<span data-ttu-id="3e212-118">说明</span><span class="sxs-lookup"><span data-stu-id="3e212-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3e212-119">列出事件</span><span class="sxs-lookup"><span data-stu-id="3e212-119">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="3e212-120">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-120">[event](event.md) collection</span></span> |<span data-ttu-id="3e212-p103">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="3e212-p103">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="3e212-123">创建事件</span><span class="sxs-lookup"><span data-stu-id="3e212-123">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="3e212-124">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-124">event</span></span>](event.md)| <span data-ttu-id="3e212-125">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-125">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="3e212-126">获取事件</span><span class="sxs-lookup"><span data-stu-id="3e212-126">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="3e212-127">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-127">event</span></span>](event.md) |<span data-ttu-id="3e212-128">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3e212-128">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="3e212-129">更新</span><span class="sxs-lookup"><span data-stu-id="3e212-129">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="3e212-130">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-130">event</span></span>](event.md) |<span data-ttu-id="3e212-131">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="3e212-131">Update event object.</span></span> |
|[<span data-ttu-id="3e212-132">删除</span><span class="sxs-lookup"><span data-stu-id="3e212-132">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="3e212-133">无</span><span class="sxs-lookup"><span data-stu-id="3e212-133">None</span></span> |<span data-ttu-id="3e212-134">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="3e212-134">Delete event object.</span></span> |
|[<span data-ttu-id="3e212-135">接受</span><span class="sxs-lookup"><span data-stu-id="3e212-135">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="3e212-136">无</span><span class="sxs-lookup"><span data-stu-id="3e212-136">None</span></span>|<span data-ttu-id="3e212-137">接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-137">Accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="3e212-138">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="3e212-138">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="3e212-139">无</span><span class="sxs-lookup"><span data-stu-id="3e212-139">None</span></span>|<span data-ttu-id="3e212-140">暂时接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-140">Tentatively accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="3e212-141">拒绝</span><span class="sxs-lookup"><span data-stu-id="3e212-141">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="3e212-142">无</span><span class="sxs-lookup"><span data-stu-id="3e212-142">None</span></span>|<span data-ttu-id="3e212-143">拒绝用户日历中的指定事件邀请。</span><span class="sxs-lookup"><span data-stu-id="3e212-143">Decline invitation to the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="3e212-144">delta</span><span class="sxs-lookup"><span data-stu-id="3e212-144">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="3e212-145">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e212-145">[event](event.md) collection</span></span>|<span data-ttu-id="3e212-146">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="3e212-146">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="3e212-147">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="3e212-147">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="3e212-148">无</span><span class="sxs-lookup"><span data-stu-id="3e212-148">None</span></span>|<span data-ttu-id="3e212-149">消除用户日历中指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="3e212-149">Dismiss the reminder for the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="3e212-150">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="3e212-150">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="3e212-151">无</span><span class="sxs-lookup"><span data-stu-id="3e212-151">None</span></span>|<span data-ttu-id="3e212-152">将用户日历中指定事件的提醒推迟至新的时间。</span><span class="sxs-lookup"><span data-stu-id="3e212-152">Postpone a reminder for the specified event in a user calendar until a new time.</span></span>|
|[<span data-ttu-id="3e212-153">列出实例</span><span class="sxs-lookup"><span data-stu-id="3e212-153">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="3e212-154">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-154">[event](event.md) collection</span></span>| <span data-ttu-id="3e212-p104">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="3e212-p104">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="3e212-157">**附件**</span><span class="sxs-lookup"><span data-stu-id="3e212-157">**Attachments**</span></span>| | |
|[<span data-ttu-id="3e212-158">列出附件</span><span class="sxs-lookup"><span data-stu-id="3e212-158">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="3e212-159">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-159">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="3e212-160">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="3e212-160">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="3e212-161">Add attachment</span><span class="sxs-lookup"><span data-stu-id="3e212-161">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="3e212-162">attachment</span><span class="sxs-lookup"><span data-stu-id="3e212-162">attachment</span></span>](attachment.md)| <span data-ttu-id="3e212-163">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="3e212-163">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="3e212-164">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="3e212-164">**Open extensions**</span></span>| | |
|[<span data-ttu-id="3e212-165">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="3e212-165">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="3e212-166">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="3e212-166">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="3e212-167">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="3e212-167">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="3e212-168">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="3e212-168">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="3e212-169">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-169">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="3e212-170">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="3e212-170">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="3e212-171">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="3e212-171">**Extended properties**</span></span>| | |
|[<span data-ttu-id="3e212-172">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="3e212-172">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="3e212-173">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-173">event</span></span>](event.md)  |<span data-ttu-id="3e212-174">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3e212-174">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="3e212-175">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="3e212-175">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3e212-176">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-176">event</span></span>](event.md) | <span data-ttu-id="3e212-177">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-177">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="3e212-178">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="3e212-178">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="3e212-179">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-179">event</span></span>](event.md) | <span data-ttu-id="3e212-180">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="3e212-180">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="3e212-181">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="3e212-181">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="3e212-182">事件</span><span class="sxs-lookup"><span data-stu-id="3e212-182">event</span></span>](event.md) | <span data-ttu-id="3e212-183">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="3e212-183">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="3e212-184">属性</span><span class="sxs-lookup"><span data-stu-id="3e212-184">Properties</span></span>
| <span data-ttu-id="3e212-185">属性</span><span class="sxs-lookup"><span data-stu-id="3e212-185">Property</span></span>     | <span data-ttu-id="3e212-186">类型</span><span class="sxs-lookup"><span data-stu-id="3e212-186">Type</span></span>   |<span data-ttu-id="3e212-187">说明</span><span class="sxs-lookup"><span data-stu-id="3e212-187">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e212-188">attendees</span><span class="sxs-lookup"><span data-stu-id="3e212-188">attendees</span></span>|<span data-ttu-id="3e212-189">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-189">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="3e212-190">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="3e212-190">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="3e212-191">body</span><span class="sxs-lookup"><span data-stu-id="3e212-191">body</span></span>|[<span data-ttu-id="3e212-192">itemBody</span><span class="sxs-lookup"><span data-stu-id="3e212-192">itemBody</span></span>](itembody.md)|<span data-ttu-id="3e212-p105">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="3e212-p105">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="3e212-195">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="3e212-195">bodyPreview</span></span>|<span data-ttu-id="3e212-196">字符串</span><span class="sxs-lookup"><span data-stu-id="3e212-196">String</span></span>|<span data-ttu-id="3e212-p106">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="3e212-p106">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="3e212-199">categories</span><span class="sxs-lookup"><span data-stu-id="3e212-199">categories</span></span>|<span data-ttu-id="3e212-200">String collection</span><span class="sxs-lookup"><span data-stu-id="3e212-200">String collection</span></span>|<span data-ttu-id="3e212-201">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="3e212-201">The categories associated with the event.</span></span>|
|<span data-ttu-id="3e212-202">changeKey</span><span class="sxs-lookup"><span data-stu-id="3e212-202">changeKey</span></span>|<span data-ttu-id="3e212-203">String</span><span class="sxs-lookup"><span data-stu-id="3e212-203">String</span></span>|<span data-ttu-id="3e212-p107">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="3e212-p107">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="3e212-207">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3e212-207">createdDateTime</span></span>|<span data-ttu-id="3e212-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e212-208">DateTimeOffset</span></span>|<span data-ttu-id="3e212-p108">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e212-p108">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e212-211">end</span><span class="sxs-lookup"><span data-stu-id="3e212-211">end</span></span>|[<span data-ttu-id="3e212-212">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e212-212">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e212-213">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3e212-213">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="3e212-214">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="3e212-214">hasAttachments</span></span>|<span data-ttu-id="3e212-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-215">Boolean</span></span>|<span data-ttu-id="3e212-216">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-216">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="3e212-217">iCalUId</span><span class="sxs-lookup"><span data-stu-id="3e212-217">iCalUId</span></span>|<span data-ttu-id="3e212-218">String</span><span class="sxs-lookup"><span data-stu-id="3e212-218">String</span></span>|<span data-ttu-id="3e212-219">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3e212-219">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="3e212-220">只读。</span><span class="sxs-lookup"><span data-stu-id="3e212-220">Read-only.</span></span>|
|<span data-ttu-id="3e212-221">id</span><span class="sxs-lookup"><span data-stu-id="3e212-221">id</span></span>|<span data-ttu-id="3e212-222">String</span><span class="sxs-lookup"><span data-stu-id="3e212-222">String</span></span>| <span data-ttu-id="3e212-223">只读。</span><span class="sxs-lookup"><span data-stu-id="3e212-223">Read-only.</span></span>|
|<span data-ttu-id="3e212-224">importance</span><span class="sxs-lookup"><span data-stu-id="3e212-224">importance</span></span>|<span data-ttu-id="3e212-225">importance</span><span class="sxs-lookup"><span data-stu-id="3e212-225">importance</span></span>|<span data-ttu-id="3e212-226">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="3e212-226">The importance of the event.</span></span> <span data-ttu-id="3e212-227">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="3e212-227">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="3e212-228">isAllDay</span><span class="sxs-lookup"><span data-stu-id="3e212-228">isAllDay</span></span>|<span data-ttu-id="3e212-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-229">Boolean</span></span>|<span data-ttu-id="3e212-230">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-230">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="3e212-231">isCancelled</span><span class="sxs-lookup"><span data-stu-id="3e212-231">isCancelled</span></span>|<span data-ttu-id="3e212-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-232">Boolean</span></span>|<span data-ttu-id="3e212-233">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-233">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="3e212-234">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="3e212-234">isOrganizer</span></span>|<span data-ttu-id="3e212-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-235">Boolean</span></span>|<span data-ttu-id="3e212-236">如果邮件发件人也是组织者，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-236">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="3e212-237">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="3e212-237">isReminderOn</span></span>|<span data-ttu-id="3e212-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-238">Boolean</span></span>|<span data-ttu-id="3e212-239">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-239">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="3e212-240">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3e212-240">lastModifiedDateTime</span></span>|<span data-ttu-id="3e212-241">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e212-241">DateTimeOffset</span></span>|<span data-ttu-id="3e212-p111">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e212-p111">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e212-244">location</span><span class="sxs-lookup"><span data-stu-id="3e212-244">location</span></span>|[<span data-ttu-id="3e212-245">位置</span><span class="sxs-lookup"><span data-stu-id="3e212-245">location</span></span>](location.md)|<span data-ttu-id="3e212-246">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="3e212-246">The location of the event.</span></span>|
|<span data-ttu-id="3e212-247">locations</span><span class="sxs-lookup"><span data-stu-id="3e212-247">locations</span></span>|<span data-ttu-id="3e212-248">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-248">[location](location.md) collection</span></span>|<span data-ttu-id="3e212-249">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="3e212-249">The locations where the event is held or attended from.</span></span> <span data-ttu-id="3e212-250">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="3e212-250">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="3e212-251">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="3e212-251">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="3e212-252">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="3e212-252">onlineMeetingUrl</span></span>|<span data-ttu-id="3e212-253">String</span><span class="sxs-lookup"><span data-stu-id="3e212-253">String</span></span>|<span data-ttu-id="3e212-254">联机会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="3e212-254">A URL for an online meeting.</span></span> <span data-ttu-id="3e212-255">仅当组织者将事件指定为联机会议（如 Skype 会议）时才会设置此属性。</span><span class="sxs-lookup"><span data-stu-id="3e212-255">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="3e212-256">只读。</span><span class="sxs-lookup"><span data-stu-id="3e212-256">Read-only.</span></span>|
|<span data-ttu-id="3e212-257">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="3e212-257">organizer</span></span>|[<span data-ttu-id="3e212-258">recipient</span><span class="sxs-lookup"><span data-stu-id="3e212-258">recipient</span></span>](recipient.md)|<span data-ttu-id="3e212-259">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="3e212-259">The organizer of the event.</span></span>|
|<span data-ttu-id="3e212-260">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e212-260">originalEndTimeZone</span></span>|<span data-ttu-id="3e212-261">String</span><span class="sxs-lookup"><span data-stu-id="3e212-261">String</span></span>|<span data-ttu-id="3e212-262">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="3e212-262">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="3e212-263">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="3e212-263">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="3e212-264">originalStart</span><span class="sxs-lookup"><span data-stu-id="3e212-264">originalStart</span></span>|<span data-ttu-id="3e212-265">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3e212-265">DateTimeOffset</span></span>|<span data-ttu-id="3e212-p115">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3e212-p115">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3e212-268">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e212-268">originalStartTimeZone</span></span>|<span data-ttu-id="3e212-269">字符串</span><span class="sxs-lookup"><span data-stu-id="3e212-269">String</span></span>|<span data-ttu-id="3e212-p116">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="3e212-p116">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="3e212-272">recurrence</span><span class="sxs-lookup"><span data-stu-id="3e212-272">recurrence</span></span>|[<span data-ttu-id="3e212-273">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="3e212-273">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="3e212-274">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="3e212-274">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="3e212-275">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="3e212-275">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="3e212-276">Int32</span><span class="sxs-lookup"><span data-stu-id="3e212-276">Int32</span></span>|<span data-ttu-id="3e212-277">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3e212-277">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="3e212-278">responseRequested</span><span class="sxs-lookup"><span data-stu-id="3e212-278">responseRequested</span></span>|<span data-ttu-id="3e212-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e212-279">Boolean</span></span>|<span data-ttu-id="3e212-280">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="3e212-280">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="3e212-281">responseStatus</span><span class="sxs-lookup"><span data-stu-id="3e212-281">responseStatus</span></span>|[<span data-ttu-id="3e212-282">responseStatus</span><span class="sxs-lookup"><span data-stu-id="3e212-282">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="3e212-283">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="3e212-283">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="3e212-284">sensitivity</span><span class="sxs-lookup"><span data-stu-id="3e212-284">sensitivity</span></span>|<span data-ttu-id="3e212-285">敏感度</span><span class="sxs-lookup"><span data-stu-id="3e212-285">sensitivity</span></span>| <span data-ttu-id="3e212-286">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="3e212-286">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="3e212-287">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="3e212-287">seriesMasterId</span></span>|<span data-ttu-id="3e212-288">String</span><span class="sxs-lookup"><span data-stu-id="3e212-288">String</span></span>|<span data-ttu-id="3e212-289">定期系列主项的 ID（如果此事件是定期系列的一部分）。</span><span class="sxs-lookup"><span data-stu-id="3e212-289">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="3e212-290">showAs</span><span class="sxs-lookup"><span data-stu-id="3e212-290">showAs</span></span>|<span data-ttu-id="3e212-291">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="3e212-291">freeBusyStatus</span></span>|<span data-ttu-id="3e212-292">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="3e212-292">The status to show.</span></span> <span data-ttu-id="3e212-293">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="3e212-293">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="3e212-294">start</span><span class="sxs-lookup"><span data-stu-id="3e212-294">start</span></span>|[<span data-ttu-id="3e212-295">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="3e212-295">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="3e212-296">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="3e212-296">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="3e212-297">subject</span><span class="sxs-lookup"><span data-stu-id="3e212-297">subject</span></span>|<span data-ttu-id="3e212-298">String</span><span class="sxs-lookup"><span data-stu-id="3e212-298">String</span></span>|<span data-ttu-id="3e212-299">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="3e212-299">The text of the event's subject line.</span></span>|
|<span data-ttu-id="3e212-300">type</span><span class="sxs-lookup"><span data-stu-id="3e212-300">type</span></span>|<span data-ttu-id="3e212-301">eventType</span><span class="sxs-lookup"><span data-stu-id="3e212-301">eventType</span></span>|<span data-ttu-id="3e212-302">事件类型。</span><span class="sxs-lookup"><span data-stu-id="3e212-302">The event type.</span></span> <span data-ttu-id="3e212-303">可能的值包括 `singleInstance`、`occurrence`、`exception`、`seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="3e212-303">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="3e212-304">只读。</span><span class="sxs-lookup"><span data-stu-id="3e212-304">Read-only.</span></span>|
|<span data-ttu-id="3e212-305">webLink</span><span class="sxs-lookup"><span data-stu-id="3e212-305">webLink</span></span>|<span data-ttu-id="3e212-306">String</span><span class="sxs-lookup"><span data-stu-id="3e212-306">String</span></span>|<span data-ttu-id="3e212-307">要在 Outlook Web App 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="3e212-307">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="3e212-p119">如果你通过 Outlook Web App 登录邮箱，该事件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="3e212-p119">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="3e212-310">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="3e212-310">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e212-311">关系</span><span class="sxs-lookup"><span data-stu-id="3e212-311">Relationships</span></span>
| <span data-ttu-id="3e212-312">关系</span><span class="sxs-lookup"><span data-stu-id="3e212-312">Relationship</span></span> | <span data-ttu-id="3e212-313">类型</span><span class="sxs-lookup"><span data-stu-id="3e212-313">Type</span></span>   |<span data-ttu-id="3e212-314">说明</span><span class="sxs-lookup"><span data-stu-id="3e212-314">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e212-315">attachments</span><span class="sxs-lookup"><span data-stu-id="3e212-315">attachments</span></span>|<span data-ttu-id="3e212-316">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-316">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="3e212-p120">事件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e212-p120">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3e212-321">日历</span><span class="sxs-lookup"><span data-stu-id="3e212-321">calendar</span></span>|[<span data-ttu-id="3e212-322">日历</span><span class="sxs-lookup"><span data-stu-id="3e212-322">calendar</span></span>](calendar.md)|<span data-ttu-id="3e212-p121">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="3e212-p121">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="3e212-326">extensions</span><span class="sxs-lookup"><span data-stu-id="3e212-326">extensions</span></span>|<span data-ttu-id="3e212-327">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="3e212-327">[Extension](extension.md) collection</span></span>|<span data-ttu-id="3e212-p122">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e212-p122">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3e212-331">instances</span><span class="sxs-lookup"><span data-stu-id="3e212-331">instances</span></span>|<span data-ttu-id="3e212-332">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-332">[event](event.md) collection</span></span>|<span data-ttu-id="3e212-p123">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e212-p123">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3e212-337">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3e212-337">multiValueExtendedProperties</span></span>|<span data-ttu-id="3e212-338">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3e212-338">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3e212-p124">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e212-p124">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="3e212-342">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="3e212-342">singleValueExtendedProperties</span></span>|<span data-ttu-id="3e212-343">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="3e212-343">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="3e212-p125">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="3e212-p125">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3e212-347">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3e212-347">JSON representation</span></span>

<span data-ttu-id="3e212-348">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3e212-348">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="3e212-349">另请参阅</span><span class="sxs-lookup"><span data-stu-id="3e212-349">See also</span></span>

- [<span data-ttu-id="3e212-350">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="3e212-350">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="3e212-351">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="3e212-351">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="3e212-352">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3e212-352">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="3e212-353">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3e212-353">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="3e212-354">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="3e212-354">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
