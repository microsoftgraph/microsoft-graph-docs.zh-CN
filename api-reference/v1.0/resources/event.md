---
title: 事件资源类型
description: 日历中的事件。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 83bacdd688705596302d7ec5c0708924a3583d20
ms.sourcegitcommit: 471f07c30867658688bd932e06822be1bbcea360
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2019
ms.locfileid: "37036191"
---
# <a name="event-resource-type"></a><span data-ttu-id="50f8d-103">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="50f8d-103">event resource type</span></span>

<span data-ttu-id="50f8d-104">[用户](user.md)日历或 Office 365 [组](group.md)日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-104">An event in a [user](user.md) calendar, or the default calendar of an Office 365 [group](group.md).</span></span>

<span data-ttu-id="50f8d-105">**事件**中包含的最大与会者人数，以及发送自 Exchange Online 邮箱的 [eventMessage](eventmessage.md) 中的收件人数上限都是 500 人。</span><span class="sxs-lookup"><span data-stu-id="50f8d-105">The maximum number of attendees included in an **event**, and the maximum number of reciepients in an [eventMessage](eventmessage.md) sent from an Exchange Online mailbox is 500.</span></span> <span data-ttu-id="50f8d-106">有关详细信息，请参阅[发送限制](https://docs.microsoft.com/zh-CN/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits)。</span><span class="sxs-lookup"><span data-stu-id="50f8d-106">For more information, see [Connector limits](https://docs.microsoft.com/zh-CN/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#sending-limits).</span></span>

<span data-ttu-id="50f8d-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="50f8d-107">This resource supports:</span></span>

- <span data-ttu-id="50f8d-108">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="50f8d-109">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="50f8d-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="50f8d-110">通过提供 [delta](../api/event-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="50f8d-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/event-delta.md) function.</span></span>

> <span data-ttu-id="50f8d-111">**注释：** 与用户日历、组日历及其事件交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="50f8d-111">**Note:** There are a few minor differences in the way you can interact with user calendars, group calendars, and their events:</span></span>

- <span data-ttu-id="50f8d-112">只可以组织 [calendarGroup](calendargroup.md) 中的用户日历。</span><span class="sxs-lookup"><span data-stu-id="50f8d-112">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="50f8d-113">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="50f8d-113">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="50f8d-114">只可以[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)_用户_日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="50f8d-114">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for _user_ calendars only.</span></span>
- <span data-ttu-id="50f8d-115">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="50f8d-115">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="50f8d-116">只可以[暂停](../api/event-snoozereminder.md)或[消除](../api/event-dismissreminder.md)_用户_日历中的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="50f8d-116">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for _user_ calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="50f8d-117">方法</span><span class="sxs-lookup"><span data-stu-id="50f8d-117">Methods</span></span>

| <span data-ttu-id="50f8d-118">方法</span><span class="sxs-lookup"><span data-stu-id="50f8d-118">Method</span></span>       | <span data-ttu-id="50f8d-119">返回类型</span><span class="sxs-lookup"><span data-stu-id="50f8d-119">Return Type</span></span>  |<span data-ttu-id="50f8d-120">说明</span><span class="sxs-lookup"><span data-stu-id="50f8d-120">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="50f8d-121">列出事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-121">List events</span></span>](../api/user-list-events.md)|<span data-ttu-id="50f8d-122">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-122">[event](event.md) collection</span></span> |<span data-ttu-id="50f8d-p104">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p104">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="50f8d-125">创建事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-125">Create event</span></span>](../api/user-post-events.md) |[<span data-ttu-id="50f8d-126">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-126">event</span></span>](event.md)| <span data-ttu-id="50f8d-127">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-127">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="50f8d-128">获取事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-128">Get event</span></span>](../api/event-get.md) | [<span data-ttu-id="50f8d-129">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-129">event</span></span>](event.md) |<span data-ttu-id="50f8d-130">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="50f8d-130">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="50f8d-131">更新</span><span class="sxs-lookup"><span data-stu-id="50f8d-131">Update</span></span>](../api/event-update.md) | [<span data-ttu-id="50f8d-132">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-132">event</span></span>](event.md) |<span data-ttu-id="50f8d-133">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="50f8d-133">Update event object.</span></span> |
|[<span data-ttu-id="50f8d-134">删除</span><span class="sxs-lookup"><span data-stu-id="50f8d-134">Delete</span></span>](../api/event-delete.md) | <span data-ttu-id="50f8d-135">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-135">None</span></span> |<span data-ttu-id="50f8d-136">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="50f8d-136">Delete event object.</span></span> |
|[<span data-ttu-id="50f8d-137">接受</span><span class="sxs-lookup"><span data-stu-id="50f8d-137">accept</span></span>](../api/event-accept.md)|<span data-ttu-id="50f8d-138">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-138">None</span></span>|<span data-ttu-id="50f8d-139">接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-139">Accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50f8d-140">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="50f8d-140">tentativelyAccept</span></span>](../api/event-tentativelyaccept.md)|<span data-ttu-id="50f8d-141">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-141">None</span></span>|<span data-ttu-id="50f8d-142">暂时接受用户日历中的指定事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-142">Tentatively accept the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50f8d-143">拒绝</span><span class="sxs-lookup"><span data-stu-id="50f8d-143">decline</span></span>](../api/event-decline.md)|<span data-ttu-id="50f8d-144">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-144">None</span></span>|<span data-ttu-id="50f8d-145">拒绝用户日历中的指定事件邀请。</span><span class="sxs-lookup"><span data-stu-id="50f8d-145">Decline invitation to the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50f8d-146">delta</span><span class="sxs-lookup"><span data-stu-id="50f8d-146">delta</span></span>](../api/event-delta.md)|<span data-ttu-id="50f8d-147">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-147">[event](event.md) collection</span></span>|<span data-ttu-id="50f8d-148">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="50f8d-148">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="50f8d-149">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="50f8d-149">dismissReminder</span></span>](../api/event-dismissreminder.md)|<span data-ttu-id="50f8d-150">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-150">None</span></span>|<span data-ttu-id="50f8d-151">消除用户日历中指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="50f8d-151">Dismiss the reminder for the specified event in a user calendar.</span></span>|
|[<span data-ttu-id="50f8d-152">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="50f8d-152">snoozeReminder</span></span>](../api/event-snoozereminder.md)|<span data-ttu-id="50f8d-153">无</span><span class="sxs-lookup"><span data-stu-id="50f8d-153">None</span></span>|<span data-ttu-id="50f8d-154">将用户日历中指定事件的提醒推迟至新的时间。</span><span class="sxs-lookup"><span data-stu-id="50f8d-154">Postpone a reminder for the specified event in a user calendar until a new time.</span></span>|
|[<span data-ttu-id="50f8d-155">列出实例</span><span class="sxs-lookup"><span data-stu-id="50f8d-155">List instances</span></span>](../api/event-list-instances.md) |<span data-ttu-id="50f8d-156">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-156">[event](event.md) collection</span></span>| <span data-ttu-id="50f8d-p105">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p105">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="50f8d-159">**附件**</span><span class="sxs-lookup"><span data-stu-id="50f8d-159">**Attachments**</span></span>| | |
|[<span data-ttu-id="50f8d-160">列出附件</span><span class="sxs-lookup"><span data-stu-id="50f8d-160">List attachments</span></span>](../api/event-list-attachments.md) |<span data-ttu-id="50f8d-161">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-161">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="50f8d-162">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-162">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="50f8d-163">Add attachment</span><span class="sxs-lookup"><span data-stu-id="50f8d-163">Add attachment</span></span>](../api/event-post-attachments.md) |[<span data-ttu-id="50f8d-164">attachment</span><span class="sxs-lookup"><span data-stu-id="50f8d-164">attachment</span></span>](attachment.md)| <span data-ttu-id="50f8d-165">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-165">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="50f8d-166">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="50f8d-166">**Open extensions**</span></span>| | |
|[<span data-ttu-id="50f8d-167">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="50f8d-167">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="50f8d-168">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="50f8d-168">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="50f8d-169">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-169">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="50f8d-170">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="50f8d-170">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="50f8d-171">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-171">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="50f8d-172">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="50f8d-172">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="50f8d-173">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="50f8d-173">**Extended properties**</span></span>| | |
|[<span data-ttu-id="50f8d-174">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="50f8d-174">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="50f8d-175">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-175">event</span></span>](event.md)  |<span data-ttu-id="50f8d-176">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-176">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="50f8d-177">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-177">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="50f8d-178">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-178">event</span></span>](event.md) | <span data-ttu-id="50f8d-179">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-179">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="50f8d-180">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="50f8d-180">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="50f8d-181">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-181">event</span></span>](event.md) | <span data-ttu-id="50f8d-182">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-182">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="50f8d-183">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-183">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="50f8d-184">事件</span><span class="sxs-lookup"><span data-stu-id="50f8d-184">event</span></span>](event.md) | <span data-ttu-id="50f8d-185">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-185">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="50f8d-186">属性</span><span class="sxs-lookup"><span data-stu-id="50f8d-186">Properties</span></span>
| <span data-ttu-id="50f8d-187">属性</span><span class="sxs-lookup"><span data-stu-id="50f8d-187">Property</span></span>     | <span data-ttu-id="50f8d-188">类型</span><span class="sxs-lookup"><span data-stu-id="50f8d-188">Type</span></span>   |<span data-ttu-id="50f8d-189">说明</span><span class="sxs-lookup"><span data-stu-id="50f8d-189">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50f8d-190">attendees</span><span class="sxs-lookup"><span data-stu-id="50f8d-190">attendees</span></span>|<span data-ttu-id="50f8d-191">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-191">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="50f8d-192">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="50f8d-192">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="50f8d-193">body</span><span class="sxs-lookup"><span data-stu-id="50f8d-193">body</span></span>|[<span data-ttu-id="50f8d-194">itemBody</span><span class="sxs-lookup"><span data-stu-id="50f8d-194">itemBody</span></span>](itembody.md)|<span data-ttu-id="50f8d-p106">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p106">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="50f8d-197">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="50f8d-197">bodyPreview</span></span>|<span data-ttu-id="50f8d-198">字符串</span><span class="sxs-lookup"><span data-stu-id="50f8d-198">String</span></span>|<span data-ttu-id="50f8d-p107">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p107">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="50f8d-201">categories</span><span class="sxs-lookup"><span data-stu-id="50f8d-201">categories</span></span>|<span data-ttu-id="50f8d-202">String collection</span><span class="sxs-lookup"><span data-stu-id="50f8d-202">String collection</span></span>|<span data-ttu-id="50f8d-203">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="50f8d-203">The categories associated with the event.</span></span>|
|<span data-ttu-id="50f8d-204">changeKey</span><span class="sxs-lookup"><span data-stu-id="50f8d-204">changeKey</span></span>|<span data-ttu-id="50f8d-205">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-205">String</span></span>|<span data-ttu-id="50f8d-p108">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p108">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="50f8d-209">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="50f8d-209">createdDateTime</span></span>|<span data-ttu-id="50f8d-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50f8d-210">DateTimeOffset</span></span>|<span data-ttu-id="50f8d-p109">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50f8d-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50f8d-213">end</span><span class="sxs-lookup"><span data-stu-id="50f8d-213">end</span></span>|[<span data-ttu-id="50f8d-214">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50f8d-214">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="50f8d-215">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="50f8d-215">The date, time, and time zone that the event ends.</span></span> <span data-ttu-id="50f8d-216">默认情况下，结束时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="50f8d-216">By default, the end time is in UTC.</span></span>|
|<span data-ttu-id="50f8d-217">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="50f8d-217">hasAttachments</span></span>|<span data-ttu-id="50f8d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-218">Boolean</span></span>|<span data-ttu-id="50f8d-219">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-219">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="50f8d-220">iCalUId</span><span class="sxs-lookup"><span data-stu-id="50f8d-220">iCalUId</span></span>|<span data-ttu-id="50f8d-221">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-221">String</span></span>|<span data-ttu-id="50f8d-222">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="50f8d-222">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="50f8d-223">只读。</span><span class="sxs-lookup"><span data-stu-id="50f8d-223">Read-only.</span></span>|
|<span data-ttu-id="50f8d-224">id</span><span class="sxs-lookup"><span data-stu-id="50f8d-224">id</span></span>|<span data-ttu-id="50f8d-225">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-225">String</span></span>| <span data-ttu-id="50f8d-226">只读。</span><span class="sxs-lookup"><span data-stu-id="50f8d-226">Read-only.</span></span>|
|<span data-ttu-id="50f8d-227">importance</span><span class="sxs-lookup"><span data-stu-id="50f8d-227">importance</span></span>|<span data-ttu-id="50f8d-228">importance</span><span class="sxs-lookup"><span data-stu-id="50f8d-228">importance</span></span>|<span data-ttu-id="50f8d-229">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-229">The importance of the event.</span></span> <span data-ttu-id="50f8d-230">可能的值包括 `low`、`normal`、`high`。</span><span class="sxs-lookup"><span data-stu-id="50f8d-230">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="50f8d-231">isAllDay</span><span class="sxs-lookup"><span data-stu-id="50f8d-231">isAllDay</span></span>|<span data-ttu-id="50f8d-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-232">Boolean</span></span>|<span data-ttu-id="50f8d-233">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-233">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="50f8d-234">isCancelled</span><span class="sxs-lookup"><span data-stu-id="50f8d-234">isCancelled</span></span>|<span data-ttu-id="50f8d-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-235">Boolean</span></span>|<span data-ttu-id="50f8d-236">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-236">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="50f8d-237">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="50f8d-237">isOrganizer</span></span>|<span data-ttu-id="50f8d-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-238">Boolean</span></span>|<span data-ttu-id="50f8d-239">如果邮件发件人也是组织者，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-239">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="50f8d-240">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="50f8d-240">isReminderOn</span></span>|<span data-ttu-id="50f8d-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-241">Boolean</span></span>|<span data-ttu-id="50f8d-242">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-242">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="50f8d-243">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="50f8d-243">lastModifiedDateTime</span></span>|<span data-ttu-id="50f8d-244">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50f8d-244">DateTimeOffset</span></span>|<span data-ttu-id="50f8d-p113">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50f8d-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50f8d-247">location</span><span class="sxs-lookup"><span data-stu-id="50f8d-247">location</span></span>|[<span data-ttu-id="50f8d-248">位置</span><span class="sxs-lookup"><span data-stu-id="50f8d-248">location</span></span>](location.md)|<span data-ttu-id="50f8d-249">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="50f8d-249">The location of the event.</span></span>|
|<span data-ttu-id="50f8d-250">locations</span><span class="sxs-lookup"><span data-stu-id="50f8d-250">locations</span></span>|<span data-ttu-id="50f8d-251">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-251">[location](location.md) collection</span></span>|<span data-ttu-id="50f8d-252">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="50f8d-252">The locations where the event is held or attended from.</span></span> <span data-ttu-id="50f8d-253">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="50f8d-253">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="50f8d-254">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="50f8d-254">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="50f8d-255">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="50f8d-255">onlineMeetingUrl</span></span>|<span data-ttu-id="50f8d-256">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-256">String</span></span>|<span data-ttu-id="50f8d-257">联机会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="50f8d-257">A URL for an online meeting.</span></span> <span data-ttu-id="50f8d-258">仅当组织者将事件指定为联机会议（如 Skype 会议）时才会设置此属性。</span><span class="sxs-lookup"><span data-stu-id="50f8d-258">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="50f8d-259">只读。</span><span class="sxs-lookup"><span data-stu-id="50f8d-259">Read-only.</span></span>|
|<span data-ttu-id="50f8d-260">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="50f8d-260">organizer</span></span>|[<span data-ttu-id="50f8d-261">recipient</span><span class="sxs-lookup"><span data-stu-id="50f8d-261">recipient</span></span>](recipient.md)|<span data-ttu-id="50f8d-262">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="50f8d-262">The organizer of the event.</span></span>|
|<span data-ttu-id="50f8d-263">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="50f8d-263">originalEndTimeZone</span></span>|<span data-ttu-id="50f8d-264">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-264">String</span></span>|<span data-ttu-id="50f8d-265">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="50f8d-265">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="50f8d-266">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="50f8d-266">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="50f8d-267">originalStart</span><span class="sxs-lookup"><span data-stu-id="50f8d-267">originalStart</span></span>|<span data-ttu-id="50f8d-268">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="50f8d-268">DateTimeOffset</span></span>|<span data-ttu-id="50f8d-p117">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="50f8d-p117">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="50f8d-271">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="50f8d-271">originalStartTimeZone</span></span>|<span data-ttu-id="50f8d-272">字符串</span><span class="sxs-lookup"><span data-stu-id="50f8d-272">String</span></span>|<span data-ttu-id="50f8d-p118">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p118">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="50f8d-275">recurrence</span><span class="sxs-lookup"><span data-stu-id="50f8d-275">recurrence</span></span>|[<span data-ttu-id="50f8d-276">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="50f8d-276">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="50f8d-277">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="50f8d-277">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="50f8d-278">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="50f8d-278">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="50f8d-279">Int32</span><span class="sxs-lookup"><span data-stu-id="50f8d-279">Int32</span></span>|<span data-ttu-id="50f8d-280">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="50f8d-280">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="50f8d-281">responseRequested</span><span class="sxs-lookup"><span data-stu-id="50f8d-281">responseRequested</span></span>|<span data-ttu-id="50f8d-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="50f8d-282">Boolean</span></span>|<span data-ttu-id="50f8d-283">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="50f8d-283">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="50f8d-284">responseStatus</span><span class="sxs-lookup"><span data-stu-id="50f8d-284">responseStatus</span></span>|[<span data-ttu-id="50f8d-285">responseStatus</span><span class="sxs-lookup"><span data-stu-id="50f8d-285">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="50f8d-286">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="50f8d-286">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="50f8d-287">sensitivity</span><span class="sxs-lookup"><span data-stu-id="50f8d-287">sensitivity</span></span>|<span data-ttu-id="50f8d-288">敏感度</span><span class="sxs-lookup"><span data-stu-id="50f8d-288">sensitivity</span></span>| <span data-ttu-id="50f8d-289">可能的值包括 `normal`、`personal`、`private`、`confidential`。</span><span class="sxs-lookup"><span data-stu-id="50f8d-289">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="50f8d-290">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="50f8d-290">seriesMasterId</span></span>|<span data-ttu-id="50f8d-291">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-291">String</span></span>|<span data-ttu-id="50f8d-292">定期系列主项的 ID（如果此事件是定期系列的一部分）。</span><span class="sxs-lookup"><span data-stu-id="50f8d-292">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="50f8d-293">showAs</span><span class="sxs-lookup"><span data-stu-id="50f8d-293">showAs</span></span>|<span data-ttu-id="50f8d-294">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="50f8d-294">freeBusyStatus</span></span>|<span data-ttu-id="50f8d-295">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="50f8d-295">The status to show.</span></span> <span data-ttu-id="50f8d-296">可能的值包括 `free`、`tentative`、`busy`、`oof`、`workingElsewhere`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="50f8d-296">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="50f8d-297">start</span><span class="sxs-lookup"><span data-stu-id="50f8d-297">start</span></span>|[<span data-ttu-id="50f8d-298">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="50f8d-298">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="50f8d-299">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="50f8d-299">The date, time, and time zone that the event starts.</span></span> <span data-ttu-id="50f8d-300">默认情况下，开始时间为 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="50f8d-300">By default, the start time is in UTC.</span></span>|
|<span data-ttu-id="50f8d-301">subject</span><span class="sxs-lookup"><span data-stu-id="50f8d-301">subject</span></span>|<span data-ttu-id="50f8d-302">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-302">String</span></span>|<span data-ttu-id="50f8d-303">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="50f8d-303">The text of the event's subject line.</span></span>|
|<span data-ttu-id="50f8d-304">type</span><span class="sxs-lookup"><span data-stu-id="50f8d-304">type</span></span>|<span data-ttu-id="50f8d-305">eventType</span><span class="sxs-lookup"><span data-stu-id="50f8d-305">eventType</span></span>|<span data-ttu-id="50f8d-306">事件类型。</span><span class="sxs-lookup"><span data-stu-id="50f8d-306">The event type.</span></span> <span data-ttu-id="50f8d-307">可能的值包括 `singleInstance`、`occurrence`、`exception`、`seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="50f8d-307">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="50f8d-308">只读。</span><span class="sxs-lookup"><span data-stu-id="50f8d-308">Read-only.</span></span>|
|<span data-ttu-id="50f8d-309">webLink</span><span class="sxs-lookup"><span data-stu-id="50f8d-309">webLink</span></span>|<span data-ttu-id="50f8d-310">String</span><span class="sxs-lookup"><span data-stu-id="50f8d-310">String</span></span>|<span data-ttu-id="50f8d-311">要在 Web 上的 Outlook 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="50f8d-311">The URL to open the event in Outlook on the web.</span></span><br/><br/><span data-ttu-id="50f8d-312">如果登录邮件，则 Outlook 网页面会在浏览器中打开事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-312">Outlook on the web opens the event in the browser if you are signed in to your mailbox.</span></span> <span data-ttu-id="50f8d-313">否则，Outlook 网页面会提示你进行登录。</span><span class="sxs-lookup"><span data-stu-id="50f8d-313">Otherwise, Outlook on the web prompts you to sign in.</span></span><br/><br/><span data-ttu-id="50f8d-314">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="50f8d-314">This URL can be accessed from within an iFrame.</span></span>|

> [!NOTE]
> <span data-ttu-id="50f8d-315">**webLink** 属性指定了一个 URL，它仅在 Outlook 网页版早期版本中打开事件。</span><span class="sxs-lookup"><span data-stu-id="50f8d-315">The **webLink** property specifies a URL that opens the event in only earlier versions of Outlook on the web.</span></span> <span data-ttu-id="50f8d-316">以下是 URL 格式，其中 _{event-id}_ 是 **id** 属性的 _**URL 编码**_ 值：</span><span class="sxs-lookup"><span data-stu-id="50f8d-316">The following are the URL formats, with _{event-id}_ being the _**URL-encoded**_ value of the **id** property:</span></span>
>
> * <span data-ttu-id="50f8d-317">对于工作或学校帐户：`https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="50f8d-317">work or school accounts`https://outlook.office365.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> * <span data-ttu-id="50f8d-318">对于 Microsoft 帐户：`https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span><span class="sxs-lookup"><span data-stu-id="50f8d-318">For Microsoft accounts: `https://outlook.live.com/owa/?itemid={event-id}&exvsurl=1&path=/calendar/item`</span></span>
>
> <span data-ttu-id="50f8d-319">要在 Outlook 网页版的当前版本中打开事件，请将 URL 转换为下述格式之一，并使用该 URL 打开事件：</span><span class="sxs-lookup"><span data-stu-id="50f8d-319">To open the event in a current version of Outlook on the web, convert the URL to one of the following formats, and use that URL to open the event:</span></span> 
>
> * <span data-ttu-id="50f8d-320">对于工作或学校帐户：`https://outlook.office365.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="50f8d-320">work or school accounts`https://outlook.office365.com/calendar/item/{event-id}`</span></span>
>
> * <span data-ttu-id="50f8d-321">对于 Microsoft 帐户：`https://outlook.live.com/calendar/item/{event-id}`</span><span class="sxs-lookup"><span data-stu-id="50f8d-321">For Microsoft accounts: `https://outlook.live.com/calendar/item/{event-id}`</span></span>


## <a name="relationships"></a><span data-ttu-id="50f8d-322">关系</span><span class="sxs-lookup"><span data-stu-id="50f8d-322">Relationships</span></span>
| <span data-ttu-id="50f8d-323">关系</span><span class="sxs-lookup"><span data-stu-id="50f8d-323">Relationship</span></span> | <span data-ttu-id="50f8d-324">类型</span><span class="sxs-lookup"><span data-stu-id="50f8d-324">Type</span></span>   |<span data-ttu-id="50f8d-325">说明</span><span class="sxs-lookup"><span data-stu-id="50f8d-325">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50f8d-326">attachments</span><span class="sxs-lookup"><span data-stu-id="50f8d-326">attachments</span></span>|<span data-ttu-id="50f8d-327">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-327">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="50f8d-p124">事件的 [fileAttachment](fileattachment.md) 和 [itemAttachment](itemattachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p124">The collection of [fileAttachment](fileattachment.md) and [itemAttachment](itemattachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50f8d-332">日历</span><span class="sxs-lookup"><span data-stu-id="50f8d-332">calendar</span></span>|[<span data-ttu-id="50f8d-333">日历</span><span class="sxs-lookup"><span data-stu-id="50f8d-333">calendar</span></span>](calendar.md)|<span data-ttu-id="50f8d-p125">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p125">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="50f8d-337">extensions</span><span class="sxs-lookup"><span data-stu-id="50f8d-337">extensions</span></span>|<span data-ttu-id="50f8d-338">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-338">[Extension](extension.md) collection</span></span>|<span data-ttu-id="50f8d-p126">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p126">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50f8d-342">instances</span><span class="sxs-lookup"><span data-stu-id="50f8d-342">instances</span></span>|<span data-ttu-id="50f8d-343">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-343">[event](event.md) collection</span></span>|<span data-ttu-id="50f8d-p127">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p127">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50f8d-348">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="50f8d-348">multiValueExtendedProperties</span></span>|<span data-ttu-id="50f8d-349">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="50f8d-349">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="50f8d-p128">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p128">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="50f8d-353">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="50f8d-353">singleValueExtendedProperties</span></span>|<span data-ttu-id="50f8d-354">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="50f8d-354">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="50f8d-p129">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="50f8d-p129">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50f8d-358">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="50f8d-358">JSON representation</span></span>

<span data-ttu-id="50f8d-359">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50f8d-359">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="50f8d-360">另请参阅</span><span class="sxs-lookup"><span data-stu-id="50f8d-360">See also</span></span>

- [<span data-ttu-id="50f8d-361">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="50f8d-361">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="50f8d-362">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="50f8d-362">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)
- [<span data-ttu-id="50f8d-363">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="50f8d-363">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="50f8d-364">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="50f8d-364">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="50f8d-365">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="50f8d-365">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
