# <a name="event-resource-type"></a><span data-ttu-id="43433-101">事件资源类型</span><span class="sxs-lookup"><span data-stu-id="43433-101">event resource type</span></span>

<span data-ttu-id="43433-102">日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="43433-102">An event in a calendar.</span></span>

<span data-ttu-id="43433-103">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="43433-103">This resource supports:</span></span>

- <span data-ttu-id="43433-104">将您自己的数据添加到自定义属性，作为[扩展](../../../concepts/extensibility_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="43433-104">Adding your own data to custom properties as [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="43433-105">订阅[更改通知](../../../concepts/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="43433-105">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="43433-106">通过提供 [delta](../api/event_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="43433-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/event_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="43433-107">方法</span><span class="sxs-lookup"><span data-stu-id="43433-107">Methods</span></span>

| <span data-ttu-id="43433-108">方法</span><span class="sxs-lookup"><span data-stu-id="43433-108">Method</span></span>       | <span data-ttu-id="43433-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="43433-109">Return Type</span></span>  |<span data-ttu-id="43433-110">说明</span><span class="sxs-lookup"><span data-stu-id="43433-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="43433-111">列出事件</span><span class="sxs-lookup"><span data-stu-id="43433-111">List events</span></span>](../api/user_list_events.md)|<span data-ttu-id="43433-112">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-112">[event](event.md) collection</span></span> |<span data-ttu-id="43433-p101">检索用户邮箱中的 [event](../resources/event.md) 对象列表。该列表包含单个实例会议和系列主控形状。</span><span class="sxs-lookup"><span data-stu-id="43433-p101">Retrieve a list of [event](../resources/event.md) objects in the user's mailbox. The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="43433-115">创建事件</span><span class="sxs-lookup"><span data-stu-id="43433-115">Create event</span></span>](../api/user_post_events.md) |[<span data-ttu-id="43433-116">事件</span><span class="sxs-lookup"><span data-stu-id="43433-116">event</span></span>](event.md)| <span data-ttu-id="43433-117">通过发布到实例集合创建新事件。</span><span class="sxs-lookup"><span data-stu-id="43433-117">Create a new event by posting to the instances collection.</span></span>|
|[<span data-ttu-id="43433-118">获取事件</span><span class="sxs-lookup"><span data-stu-id="43433-118">Get event</span></span>](../api/event_get.md) | [<span data-ttu-id="43433-119">事件</span><span class="sxs-lookup"><span data-stu-id="43433-119">event</span></span>](event.md) |<span data-ttu-id="43433-120">读取 event 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="43433-120">Read properties and relationships of event object.</span></span>|
|[<span data-ttu-id="43433-121">更新</span><span class="sxs-lookup"><span data-stu-id="43433-121">Update</span></span>](../api/event_update.md) | [<span data-ttu-id="43433-122">事件</span><span class="sxs-lookup"><span data-stu-id="43433-122">event</span></span>](event.md) |<span data-ttu-id="43433-123">更新事件对象。</span><span class="sxs-lookup"><span data-stu-id="43433-123">Update event object.</span></span> |
|[<span data-ttu-id="43433-124">删除</span><span class="sxs-lookup"><span data-stu-id="43433-124">Delete</span></span>](../api/event_delete.md) | <span data-ttu-id="43433-125">无</span><span class="sxs-lookup"><span data-stu-id="43433-125">None</span></span> |<span data-ttu-id="43433-126">删除事件对象。</span><span class="sxs-lookup"><span data-stu-id="43433-126">Delete event object.</span></span> |
|[<span data-ttu-id="43433-127">接受</span><span class="sxs-lookup"><span data-stu-id="43433-127">accept</span></span>](../api/event_accept.md)|<span data-ttu-id="43433-128">无</span><span class="sxs-lookup"><span data-stu-id="43433-128">None</span></span>|<span data-ttu-id="43433-129">接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="43433-129">Accept the specified event.</span></span>|
|[<span data-ttu-id="43433-130">tentativelyAccept</span><span class="sxs-lookup"><span data-stu-id="43433-130">tentativelyAccept</span></span>](../api/event_tentativelyaccept.md)|<span data-ttu-id="43433-131">无</span><span class="sxs-lookup"><span data-stu-id="43433-131">None</span></span>|<span data-ttu-id="43433-132">暂时接受指定的事件。</span><span class="sxs-lookup"><span data-stu-id="43433-132">Tentatively accept the specified event.</span></span>|
|[<span data-ttu-id="43433-133">拒绝</span><span class="sxs-lookup"><span data-stu-id="43433-133">decline</span></span>](../api/event_decline.md)|<span data-ttu-id="43433-134">无</span><span class="sxs-lookup"><span data-stu-id="43433-134">None</span></span>|<span data-ttu-id="43433-135">拒绝对指定事件的邀请。</span><span class="sxs-lookup"><span data-stu-id="43433-135">Decline invitation to the specified event.</span></span>|
|[<span data-ttu-id="43433-136">delta</span><span class="sxs-lookup"><span data-stu-id="43433-136">delta</span></span>](../api/event_delta.md)|<span data-ttu-id="43433-137">[事件](event.md)集合</span><span class="sxs-lookup"><span data-stu-id="43433-137">[event](event.md) collection</span></span>|<span data-ttu-id="43433-138">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="43433-138">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>|
|[<span data-ttu-id="43433-139">dismissReminder</span><span class="sxs-lookup"><span data-stu-id="43433-139">dismissReminder</span></span>](../api/event_dismissreminder.md)|<span data-ttu-id="43433-140">无</span><span class="sxs-lookup"><span data-stu-id="43433-140">None</span></span>|<span data-ttu-id="43433-141">消除指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="43433-141">Dismiss the reminder for the specified event.</span></span>|
|[<span data-ttu-id="43433-142">snoozeReminder</span><span class="sxs-lookup"><span data-stu-id="43433-142">snoozeReminder</span></span>](../api/event_snoozereminder.md)|<span data-ttu-id="43433-143">无</span><span class="sxs-lookup"><span data-stu-id="43433-143">None</span></span>|<span data-ttu-id="43433-144">暂停指定事件的提醒。</span><span class="sxs-lookup"><span data-stu-id="43433-144">Snooze the reminder for the specified event.</span></span>|
|[<span data-ttu-id="43433-145">列出实例</span><span class="sxs-lookup"><span data-stu-id="43433-145">List instances</span></span>](../api/event_list_instances.md) |<span data-ttu-id="43433-146">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-146">[event](event.md) collection</span></span>| <span data-ttu-id="43433-p102">获取指定的时间范围的事件的实例（发生次数）。如果事件的类型是 `SeriesMaster`，这将返回在指定的时间范围内事件的发生次数和异常。</span><span class="sxs-lookup"><span data-stu-id="43433-p102">Get the instances (occurrences) of an event for a specified time range. If the event is a `SeriesMaster` type, this returns the occurrences and exceptions of the event in the specified time range.</span></span>|
|<span data-ttu-id="43433-149">**附件**</span><span class="sxs-lookup"><span data-stu-id="43433-149">**Attachments**</span></span>| | |
|[<span data-ttu-id="43433-150">列出附件</span><span class="sxs-lookup"><span data-stu-id="43433-150">List attachments</span></span>](../api/event_list_attachments.md) |<span data-ttu-id="43433-151">[attachment](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-151">[attachment](attachment.md) collection</span></span>| <span data-ttu-id="43433-152">获取事件的所有附件。</span><span class="sxs-lookup"><span data-stu-id="43433-152">Get all attachments on an event.</span></span>|
|[<span data-ttu-id="43433-153">Add attachment</span><span class="sxs-lookup"><span data-stu-id="43433-153">Add attachment</span></span>](../api/event_post_attachments.md) |[<span data-ttu-id="43433-154">attachment</span><span class="sxs-lookup"><span data-stu-id="43433-154">attachment</span></span>](attachment.md)| <span data-ttu-id="43433-155">通过发布到附件集合，向事件添加新附件。</span><span class="sxs-lookup"><span data-stu-id="43433-155">Add a new attachment to an event by posting to the attachments collection.</span></span>|
|<span data-ttu-id="43433-156">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="43433-156">**Open extensions**</span></span>| | |
|[<span data-ttu-id="43433-157">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="43433-157">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="43433-158">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="43433-158">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="43433-159">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="43433-159">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="43433-160">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="43433-160">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="43433-161">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-161">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="43433-162">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="43433-162">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="43433-163">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="43433-163">**Extended properties**</span></span>| | |
|[<span data-ttu-id="43433-164">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="43433-164">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="43433-165">事件</span><span class="sxs-lookup"><span data-stu-id="43433-165">event</span></span>](event.md)  |<span data-ttu-id="43433-166">在新建或现有事件中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="43433-166">Create one or more single-value extended properties in a new or existing event.</span></span>   |
|[<span data-ttu-id="43433-167">获取具有单值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="43433-167">Get event with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="43433-168">事件</span><span class="sxs-lookup"><span data-stu-id="43433-168">event</span></span>](event.md) | <span data-ttu-id="43433-169">通过使用 `$expand` 或 `$filter` 获取包含单值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="43433-169">Get events that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="43433-170">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="43433-170">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="43433-171">事件</span><span class="sxs-lookup"><span data-stu-id="43433-171">event</span></span>](event.md) | <span data-ttu-id="43433-172">在新建或现有的事件中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="43433-172">Create one or more multi-value extended properties in a new or existing event.</span></span>  |
|[<span data-ttu-id="43433-173">获取具有多值扩展属性的事件</span><span class="sxs-lookup"><span data-stu-id="43433-173">Get event with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="43433-174">事件</span><span class="sxs-lookup"><span data-stu-id="43433-174">event</span></span>](event.md) | <span data-ttu-id="43433-175">使用 `$expand` 获取包含一个多值扩展属性的事件。</span><span class="sxs-lookup"><span data-stu-id="43433-175">Get an event that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="43433-176">属性</span><span class="sxs-lookup"><span data-stu-id="43433-176">Properties</span></span>
| <span data-ttu-id="43433-177">属性</span><span class="sxs-lookup"><span data-stu-id="43433-177">Property</span></span>     | <span data-ttu-id="43433-178">类型</span><span class="sxs-lookup"><span data-stu-id="43433-178">Type</span></span>   |<span data-ttu-id="43433-179">说明</span><span class="sxs-lookup"><span data-stu-id="43433-179">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43433-180">attendees</span><span class="sxs-lookup"><span data-stu-id="43433-180">attendees</span></span>|<span data-ttu-id="43433-181">[与会者](attendee.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-181">[attendee](attendee.md) collection</span></span>|<span data-ttu-id="43433-182">事件的与会者集合。</span><span class="sxs-lookup"><span data-stu-id="43433-182">The collection of attendees for the event.</span></span>|
|<span data-ttu-id="43433-183">body</span><span class="sxs-lookup"><span data-stu-id="43433-183">body</span></span>|[<span data-ttu-id="43433-184">itemBody</span><span class="sxs-lookup"><span data-stu-id="43433-184">itemBody</span></span>](itembody.md)|<span data-ttu-id="43433-p103">与事件相关联的邮件正文。可以是 HTML 格式或文本格式。</span><span class="sxs-lookup"><span data-stu-id="43433-p103">The body of the message associated with the event. It can be in HTML or text format.</span></span>|
|<span data-ttu-id="43433-187">bodyPreview</span><span class="sxs-lookup"><span data-stu-id="43433-187">bodyPreview</span></span>|<span data-ttu-id="43433-188">字符串</span><span class="sxs-lookup"><span data-stu-id="43433-188">String</span></span>|<span data-ttu-id="43433-p104">与事件相关联的邮件预览。文本格式。</span><span class="sxs-lookup"><span data-stu-id="43433-p104">The preview of the message associated with the event. It is in text format.</span></span>|
|<span data-ttu-id="43433-191">categories</span><span class="sxs-lookup"><span data-stu-id="43433-191">categories</span></span>|<span data-ttu-id="43433-192">String collection</span><span class="sxs-lookup"><span data-stu-id="43433-192">String collection</span></span>|<span data-ttu-id="43433-193">与事件相关联的类别。</span><span class="sxs-lookup"><span data-stu-id="43433-193">The categories associated with the event.</span></span>|
|<span data-ttu-id="43433-194">changeKey</span><span class="sxs-lookup"><span data-stu-id="43433-194">changeKey</span></span>|<span data-ttu-id="43433-195">String</span><span class="sxs-lookup"><span data-stu-id="43433-195">String</span></span>|<span data-ttu-id="43433-p105">标识 event 对象的版本。每次事件更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="43433-p105">Identifies the version of the event object. Every time the event is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="43433-199">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="43433-199">createdDateTime</span></span>|<span data-ttu-id="43433-200">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43433-200">DateTimeOffset</span></span>|<span data-ttu-id="43433-p106">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="43433-p106">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="43433-203">end</span><span class="sxs-lookup"><span data-stu-id="43433-203">end</span></span>|[<span data-ttu-id="43433-204">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="43433-204">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="43433-205">事件结束的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="43433-205">The date, time, and time zone that the event ends.</span></span>|
|<span data-ttu-id="43433-206">hasAttachments</span><span class="sxs-lookup"><span data-stu-id="43433-206">hasAttachments</span></span>|<span data-ttu-id="43433-207">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-207">Boolean</span></span>|<span data-ttu-id="43433-208">如果事件包含附件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-208">Set to true if the event has attachments.</span></span>|
|<span data-ttu-id="43433-209">iCalUId</span><span class="sxs-lookup"><span data-stu-id="43433-209">iCalUId</span></span>|<span data-ttu-id="43433-210">String</span><span class="sxs-lookup"><span data-stu-id="43433-210">String</span></span>|<span data-ttu-id="43433-211">由不同日历间的所有事件实例共享的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="43433-211">A unique identifier that is shared by all instances of an event across different calendars.</span></span> <span data-ttu-id="43433-212">只读。</span><span class="sxs-lookup"><span data-stu-id="43433-212">Read-only.</span></span>|
|<span data-ttu-id="43433-213">id</span><span class="sxs-lookup"><span data-stu-id="43433-213">id</span></span>|<span data-ttu-id="43433-214">String</span><span class="sxs-lookup"><span data-stu-id="43433-214">String</span></span>| <span data-ttu-id="43433-215">只读。</span><span class="sxs-lookup"><span data-stu-id="43433-215">Read-only.</span></span>|
|<span data-ttu-id="43433-216">importance</span><span class="sxs-lookup"><span data-stu-id="43433-216">importance</span></span>|<span data-ttu-id="43433-217">importance</span><span class="sxs-lookup"><span data-stu-id="43433-217">importance</span></span>|<span data-ttu-id="43433-218">事件的重要性。</span><span class="sxs-lookup"><span data-stu-id="43433-218">The importance of the event.</span></span> <span data-ttu-id="43433-219">可能的值为： `low`， `normal`， `high`。</span><span class="sxs-lookup"><span data-stu-id="43433-219">The possible values are: `low`, `normal`, `high`.</span></span>|
|<span data-ttu-id="43433-220">isAllDay</span><span class="sxs-lookup"><span data-stu-id="43433-220">isAllDay</span></span>|<span data-ttu-id="43433-221">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-221">Boolean</span></span>|<span data-ttu-id="43433-222">如果事件持续一整天，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-222">Set to true if the event lasts all day.</span></span>|
|<span data-ttu-id="43433-223">isCancelled</span><span class="sxs-lookup"><span data-stu-id="43433-223">isCancelled</span></span>|<span data-ttu-id="43433-224">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-224">Boolean</span></span>|<span data-ttu-id="43433-225">如果事件已取消，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-225">Set to true if the event has been canceled.</span></span>|
|<span data-ttu-id="43433-226">isOrganizer</span><span class="sxs-lookup"><span data-stu-id="43433-226">isOrganizer</span></span>|<span data-ttu-id="43433-227">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-227">Boolean</span></span>|<span data-ttu-id="43433-228">如果邮件发件人也是组织者，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-228">Set to true if the message sender is also the organizer.</span></span>|
|<span data-ttu-id="43433-229">isReminderOn</span><span class="sxs-lookup"><span data-stu-id="43433-229">isReminderOn</span></span>|<span data-ttu-id="43433-230">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-230">Boolean</span></span>|<span data-ttu-id="43433-231">如果设置警报以提醒用户有事件，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-231">Set to true if an alert is set to remind the user of the event.</span></span>|
|<span data-ttu-id="43433-232">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="43433-232">lastModifiedDateTime</span></span>|<span data-ttu-id="43433-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43433-233">DateTimeOffset</span></span>|<span data-ttu-id="43433-p109">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="43433-p109">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="43433-236">location</span><span class="sxs-lookup"><span data-stu-id="43433-236">location</span></span>|[<span data-ttu-id="43433-237">位置</span><span class="sxs-lookup"><span data-stu-id="43433-237">location</span></span>](location.md)|<span data-ttu-id="43433-238">事件的位置。</span><span class="sxs-lookup"><span data-stu-id="43433-238">The location of the event.</span></span>|
|<span data-ttu-id="43433-239">locations</span><span class="sxs-lookup"><span data-stu-id="43433-239">locations</span></span>|<span data-ttu-id="43433-240">[location](location.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-240">[location](location.md) collection</span></span>|<span data-ttu-id="43433-241">举办或参加活动的地点。</span><span class="sxs-lookup"><span data-stu-id="43433-241">The locations where the event is held or attended from.</span></span> <span data-ttu-id="43433-242">**location** 和 **locations** 属性总是相互对应。</span><span class="sxs-lookup"><span data-stu-id="43433-242">The **location** and **locations** properties always correspond with each other.</span></span> <span data-ttu-id="43433-243">如果更新 **location** 属性，**locations** 集合中所有以前的位置都将被删除并替换为新的 **location** 值。</span><span class="sxs-lookup"><span data-stu-id="43433-243">If you update the **location** property, any prior locations in the **locations** collection would be removed and replaced by the new **location** value.</span></span> |
|<span data-ttu-id="43433-244">onlineMeetingUrl</span><span class="sxs-lookup"><span data-stu-id="43433-244">onlineMeetingUrl</span></span>|<span data-ttu-id="43433-245">String</span><span class="sxs-lookup"><span data-stu-id="43433-245">String</span></span>|<span data-ttu-id="43433-246">在线会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="43433-246">A URL for an online meeting.</span></span> <span data-ttu-id="43433-247">仅组织者指定为联机会议如 Skype 会议事件时，该属性是设置。</span><span class="sxs-lookup"><span data-stu-id="43433-247">The property is set only when an organizer specifies an event as an online meeting such as a Skype meeting.</span></span> <span data-ttu-id="43433-248">只读。</span><span class="sxs-lookup"><span data-stu-id="43433-248">Read-only.</span></span>|
|<span data-ttu-id="43433-249">organizer</span><span class="sxs-lookup"><span data-stu-id="43433-249">organizer</span></span>|[<span data-ttu-id="43433-250">recipient</span><span class="sxs-lookup"><span data-stu-id="43433-250">recipient</span></span>](recipient.md)|<span data-ttu-id="43433-251">事件的组织者。</span><span class="sxs-lookup"><span data-stu-id="43433-251">The organizer of the event.</span></span>|
|<span data-ttu-id="43433-252">originalEndTimeZone</span><span class="sxs-lookup"><span data-stu-id="43433-252">originalEndTimeZone</span></span>|<span data-ttu-id="43433-253">String</span><span class="sxs-lookup"><span data-stu-id="43433-253">String</span></span>|<span data-ttu-id="43433-254">创建事件时设置的结束时区。</span><span class="sxs-lookup"><span data-stu-id="43433-254">The end time zone that was set when the event was created.</span></span> <span data-ttu-id="43433-255">`tzone://Microsoft/Custom` 值表示旧的自定义时区已在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="43433-255">A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span>|
|<span data-ttu-id="43433-256">originalStart</span><span class="sxs-lookup"><span data-stu-id="43433-256">originalStart</span></span>|<span data-ttu-id="43433-257">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="43433-257">DateTimeOffset</span></span>|<span data-ttu-id="43433-p113">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="43433-p113">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="43433-260">originalStartTimeZone</span><span class="sxs-lookup"><span data-stu-id="43433-260">originalStartTimeZone</span></span>|<span data-ttu-id="43433-261">字符串</span><span class="sxs-lookup"><span data-stu-id="43433-261">String</span></span>|<span data-ttu-id="43433-p114">创建事件时设置的开始时区。`tzone://Microsoft/Custom` 值表示旧的自定义时区在桌面版 Outlook 中设置。</span><span class="sxs-lookup"><span data-stu-id="43433-p114">The start time zone that was set when the event was created. A value of `tzone://Microsoft/Custom` indicates that a legacy custom time zone was set in desktop Outlook.</span></span> |
|<span data-ttu-id="43433-264">recurrence</span><span class="sxs-lookup"><span data-stu-id="43433-264">recurrence</span></span>|[<span data-ttu-id="43433-265">patternedRecurrence</span><span class="sxs-lookup"><span data-stu-id="43433-265">patternedRecurrence</span></span>](patternedrecurrence.md)|<span data-ttu-id="43433-266">事件的定期模式。</span><span class="sxs-lookup"><span data-stu-id="43433-266">The recurrence pattern for the event.</span></span>|
|<span data-ttu-id="43433-267">reminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="43433-267">reminderMinutesBeforeStart</span></span>|<span data-ttu-id="43433-268">Int32</span><span class="sxs-lookup"><span data-stu-id="43433-268">Int32</span></span>|<span data-ttu-id="43433-269">事件开始时间（即提醒警报发生时间）之前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="43433-269">The number of minutes before the event start time that the reminder alert occurs.</span></span>|
|<span data-ttu-id="43433-270">responseRequested</span><span class="sxs-lookup"><span data-stu-id="43433-270">responseRequested</span></span>|<span data-ttu-id="43433-271">布尔</span><span class="sxs-lookup"><span data-stu-id="43433-271">Boolean</span></span>|<span data-ttu-id="43433-272">如果发件人希望接收事件被接受或拒绝时的响应，则设置为 true。</span><span class="sxs-lookup"><span data-stu-id="43433-272">Set to true if the sender would like a response when the event is accepted or declined.</span></span>|
|<span data-ttu-id="43433-273">responseStatus</span><span class="sxs-lookup"><span data-stu-id="43433-273">responseStatus</span></span>|[<span data-ttu-id="43433-274">responseStatus</span><span class="sxs-lookup"><span data-stu-id="43433-274">responseStatus</span></span>](responsestatus.md)|<span data-ttu-id="43433-275">指示在事件消息的响应中发送的响应类型。</span><span class="sxs-lookup"><span data-stu-id="43433-275">Indicates the type of response sent in response to an event message.</span></span>|
|<span data-ttu-id="43433-276">sensitivity</span><span class="sxs-lookup"><span data-stu-id="43433-276">sensitivity</span></span>|<span data-ttu-id="43433-277">sensitivity</span><span class="sxs-lookup"><span data-stu-id="43433-277">sensitivity</span></span>| <span data-ttu-id="43433-278">可能的值为： `normal`， `personal`， `private`， `confidential`。</span><span class="sxs-lookup"><span data-stu-id="43433-278">The possible values are: `normal`, `personal`, `private`, `confidential`.</span></span>|
|<span data-ttu-id="43433-279">seriesMasterId</span><span class="sxs-lookup"><span data-stu-id="43433-279">seriesMasterId</span></span>|<span data-ttu-id="43433-280">String</span><span class="sxs-lookup"><span data-stu-id="43433-280">String</span></span>|<span data-ttu-id="43433-281">定期系列主项目，如果该事件是定期系列的一部分的 ID。</span><span class="sxs-lookup"><span data-stu-id="43433-281">The ID for the recurring series master item, if this event is part of a recurring series.</span></span>|
|<span data-ttu-id="43433-282">showAs</span><span class="sxs-lookup"><span data-stu-id="43433-282">showAs</span></span>|<span data-ttu-id="43433-283">freeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="43433-283">freeBusyStatus</span></span>|<span data-ttu-id="43433-284">要显示的状态。</span><span class="sxs-lookup"><span data-stu-id="43433-284">The status to show.</span></span> <span data-ttu-id="43433-285">可能的值为： `free`， `tentative`， `busy`， `oof`， `workingElsewhere`， `unknown`。</span><span class="sxs-lookup"><span data-stu-id="43433-285">The possible values are: `free`, `tentative`, `busy`, `oof`, `workingElsewhere`, `unknown`.</span></span>|
|<span data-ttu-id="43433-286">start</span><span class="sxs-lookup"><span data-stu-id="43433-286">start</span></span>|[<span data-ttu-id="43433-287">dateTimeTimeZone</span><span class="sxs-lookup"><span data-stu-id="43433-287">dateTimeTimeZone</span></span>](datetimetimezone.md)|<span data-ttu-id="43433-288">事件开始的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="43433-288">The date, time, and time zone that the event starts.</span></span>|
|<span data-ttu-id="43433-289">subject</span><span class="sxs-lookup"><span data-stu-id="43433-289">subject</span></span>|<span data-ttu-id="43433-290">String</span><span class="sxs-lookup"><span data-stu-id="43433-290">String</span></span>|<span data-ttu-id="43433-291">事件的主题行文本。</span><span class="sxs-lookup"><span data-stu-id="43433-291">The text of the event's subject line.</span></span>|
|<span data-ttu-id="43433-292">type</span><span class="sxs-lookup"><span data-stu-id="43433-292">type</span></span>|<span data-ttu-id="43433-293">eventType</span><span class="sxs-lookup"><span data-stu-id="43433-293">eventType</span></span>|<span data-ttu-id="43433-294">事件类型。</span><span class="sxs-lookup"><span data-stu-id="43433-294">The event type.</span></span> <span data-ttu-id="43433-295">可能的值为： `singleInstance`， `occurrence`， `exception`， `seriesMaster`。</span><span class="sxs-lookup"><span data-stu-id="43433-295">The possible values are: `singleInstance`, `occurrence`, `exception`, `seriesMaster`.</span></span> <span data-ttu-id="43433-296">只读。</span><span class="sxs-lookup"><span data-stu-id="43433-296">Read-only.</span></span>|
|<span data-ttu-id="43433-297">webLink</span><span class="sxs-lookup"><span data-stu-id="43433-297">webLink</span></span>|<span data-ttu-id="43433-298">String</span><span class="sxs-lookup"><span data-stu-id="43433-298">String</span></span>|<span data-ttu-id="43433-299">要在 Outlook Web App 中打开事件的 URL。</span><span class="sxs-lookup"><span data-stu-id="43433-299">The URL to open the event in Outlook Web App.</span></span><br/><br/><span data-ttu-id="43433-p117">如果你通过 Outlook Web App 登录邮箱，该事件将在浏览器中打开。如果尚未使用浏览器登录，系统将提示你登录。</span><span class="sxs-lookup"><span data-stu-id="43433-p117">The event will open in the browser if you are logged in to your mailbox via Outlook Web App. You will be prompted to login if you are not already logged in with the browser.</span></span><br/><br/><span data-ttu-id="43433-302">可以从 iFrame 中访问此 URL。</span><span class="sxs-lookup"><span data-stu-id="43433-302">This URL can be accessed from within an iFrame.</span></span>|

## <a name="relationships"></a><span data-ttu-id="43433-303">关系</span><span class="sxs-lookup"><span data-stu-id="43433-303">Relationships</span></span>
| <span data-ttu-id="43433-304">关系</span><span class="sxs-lookup"><span data-stu-id="43433-304">Relationship</span></span> | <span data-ttu-id="43433-305">类型</span><span class="sxs-lookup"><span data-stu-id="43433-305">Type</span></span>   |<span data-ttu-id="43433-306">说明</span><span class="sxs-lookup"><span data-stu-id="43433-306">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43433-307">attachments</span><span class="sxs-lookup"><span data-stu-id="43433-307">attachments</span></span>|<span data-ttu-id="43433-308">[附件](attachment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-308">[attachment](attachment.md) collection</span></span>|<span data-ttu-id="43433-p118">事件的 [fileAttachment](fileAttachment.md) 和 [itemAttachment](itemAttachment.md) 附件集合。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="43433-p118">The collection of [fileAttachment](fileAttachment.md) and [itemAttachment](itemAttachment.md) attachments for the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="43433-313">日历</span><span class="sxs-lookup"><span data-stu-id="43433-313">calendar</span></span>|[<span data-ttu-id="43433-314">日历</span><span class="sxs-lookup"><span data-stu-id="43433-314">calendar</span></span>](calendar.md)|<span data-ttu-id="43433-p119">包含事件的日历。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="43433-p119">The calendar that contains the event. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="43433-318">extensions</span><span class="sxs-lookup"><span data-stu-id="43433-318">extensions</span></span>|<span data-ttu-id="43433-319">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="43433-319">[Extension](extension.md) collection</span></span>|<span data-ttu-id="43433-p120">为事件定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="43433-p120">The collection of open extensions defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="43433-323">instances</span><span class="sxs-lookup"><span data-stu-id="43433-323">instances</span></span>|<span data-ttu-id="43433-324">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-324">[event](event.md) collection</span></span>|<span data-ttu-id="43433-p121">事件的实例。导航属性。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="43433-p121">The instances of the event. Navigation property. Read-only. Nullable.</span></span>|
|<span data-ttu-id="43433-329">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="43433-329">multiValueExtendedProperties</span></span>|<span data-ttu-id="43433-330">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="43433-330">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="43433-p122">为事件定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="43433-p122">The collection of multi-value extended properties defined for the event. Read-only. Nullable.</span></span>|
|<span data-ttu-id="43433-334">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="43433-334">singleValueExtendedProperties</span></span>|<span data-ttu-id="43433-335">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="43433-335">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="43433-p123">为事件定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="43433-p123">The collection of single-value extended properties defined for the event. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43433-339">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43433-339">JSON representation</span></span>

<span data-ttu-id="43433-340">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43433-340">Here is a JSON representation of the resource</span></span>

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


## <a name="see-also"></a><span data-ttu-id="43433-341">另请参阅</span><span class="sxs-lookup"><span data-stu-id="43433-341">See also</span></span>

- [<span data-ttu-id="43433-342">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="43433-342">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="43433-343">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="43433-343">Get incremental changes to events in a folder</span></span>](../../../concepts/delta_query_events.md)
- [<span data-ttu-id="43433-344">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="43433-344">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="43433-345">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="43433-345">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="43433-346">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="43433-346">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "event resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
