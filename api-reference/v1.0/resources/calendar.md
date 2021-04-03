---
title: 日历资源类型
description: 日历即事件容器。 它可以是用户的日历，或者是 Microsoft 365 组的默认日历。
localization_priority: Priority
author: harini84
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: cdbae695cff9469f31d4a2e813312a9608e3bb98
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509315"
---
# <a name="calendar-resource-type"></a><span data-ttu-id="8a834-104">日历资源类型</span><span class="sxs-lookup"><span data-stu-id="8a834-104">calendar resource type</span></span>

<span data-ttu-id="8a834-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a834-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8a834-106">表示[事件](event.md)资源的容器。</span><span class="sxs-lookup"><span data-stu-id="8a834-106">Represents a container for [event](event.md) resources.</span></span> <span data-ttu-id="8a834-107">它可以是 [用户](user.md)的日历，或者 Microsoft 365 [组](group.md)的默认日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-107">It can be a calendar for a [user](user.md), or the default calendar of a Microsoft 365 [group](group.md).</span></span>

> <span data-ttu-id="8a834-108">**注意：** 与用户日历和组日历交互的方式稍有不同：</span><span class="sxs-lookup"><span data-stu-id="8a834-108">**Note:** There are a few minor differences in the way you can interact with user calendars and group calendars:</span></span>

- <span data-ttu-id="8a834-109">只能将用户日历组织到 [calendarGroup](calendargroup.md) 中。</span><span class="sxs-lookup"><span data-stu-id="8a834-109">You can organize only user calendars in a [calendarGroup](calendargroup.md).</span></span>
- <span data-ttu-id="8a834-110">Outlook 将代表组自动接受所有会议请求。</span><span class="sxs-lookup"><span data-stu-id="8a834-110">Outlook automatically accepts all meeting requests on behalf of groups.</span></span> <span data-ttu-id="8a834-111">只能[接受](../api/event-accept.md)、[暂时接受](../api/event-tentativelyaccept.md)或[拒绝](../api/event-decline.md)用户日历中的会议请求。</span><span class="sxs-lookup"><span data-stu-id="8a834-111">You can [accept](../api/event-accept.md), [tentatively accept](../api/event-tentativelyaccept.md), or [decline](../api/event-decline.md)  meeting requests for user calendars only.</span></span>
- <span data-ttu-id="8a834-112">Outlook 不支持对组事件提供提醒。</span><span class="sxs-lookup"><span data-stu-id="8a834-112">Outlook doesn't support reminders for group events.</span></span> <span data-ttu-id="8a834-113">只能[推迟](../api/event-snoozereminder.md)或[取消](../api/event-dismissreminder.md)用户日历的[提醒](reminder.md)。</span><span class="sxs-lookup"><span data-stu-id="8a834-113">You can [snooze](../api/event-snoozereminder.md) or [dismiss](../api/event-dismissreminder.md) a [reminder](reminder.md) for user calendars only.</span></span>

## <a name="methods"></a><span data-ttu-id="8a834-114">方法</span><span class="sxs-lookup"><span data-stu-id="8a834-114">Methods</span></span>

| <span data-ttu-id="8a834-115">方法</span><span class="sxs-lookup"><span data-stu-id="8a834-115">Method</span></span>       | <span data-ttu-id="8a834-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="8a834-116">Return Type</span></span>  |<span data-ttu-id="8a834-117">说明</span><span class="sxs-lookup"><span data-stu-id="8a834-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8a834-118">列出日历</span><span class="sxs-lookup"><span data-stu-id="8a834-118">List calendars</span></span>](../api/user-list-calendars.md)|<span data-ttu-id="8a834-119">[日历](calendar.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-119">[calendar](calendar.md) collection</span></span>|<span data-ttu-id="8a834-120">获取所有用户的日历，或者获取默认或其他特定日历组中的日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-120">Get all the user's calendars, or the calendars in the default or other specific calendar group.</span></span>|
|[<span data-ttu-id="8a834-121">创建日历</span><span class="sxs-lookup"><span data-stu-id="8a834-121">Create calendar</span></span>](../api/user-post-calendars.md) |[<span data-ttu-id="8a834-122">calendar</span><span class="sxs-lookup"><span data-stu-id="8a834-122">calendar</span></span>](calendar.md)| <span data-ttu-id="8a834-123">在默认日历组或用户的指定日历组中新建日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-123">Create a new calendar in the default calendar group or specified calendar group for a user.</span></span>|
|[<span data-ttu-id="8a834-124">Get calendar</span><span class="sxs-lookup"><span data-stu-id="8a834-124">Get calendar</span></span>](../api/calendar-get.md) | [<span data-ttu-id="8a834-125">calendar</span><span class="sxs-lookup"><span data-stu-id="8a834-125">calendar</span></span>](calendar.md) |<span data-ttu-id="8a834-126">获取 **calendar** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8a834-126">Get the properties and relationships of a **calendar** object.</span></span> <span data-ttu-id="8a834-127">可以是用户的日历，也可以是 Microsoft 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-127">The calendar can be one for a user, or the default calendar of a Microsoft 365 group.</span></span> |
|[<span data-ttu-id="8a834-128">更新</span><span class="sxs-lookup"><span data-stu-id="8a834-128">Update</span></span>](../api/calendar-update.md) | [<span data-ttu-id="8a834-129">calendar</span><span class="sxs-lookup"><span data-stu-id="8a834-129">calendar</span></span>](calendar.md)  |<span data-ttu-id="8a834-130">更新 **calendar** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8a834-130">Update the properties of a **calendar** object.</span></span> <span data-ttu-id="8a834-131">可以是用户的日历，也可以是 Microsoft 365 组的默认日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-131">The calendar can be one for a user, or the default calendar of a Microsoft 365 group.</span></span> |
|[<span data-ttu-id="8a834-132">删除</span><span class="sxs-lookup"><span data-stu-id="8a834-132">Delete</span></span>](../api/calendar-delete.md) | <span data-ttu-id="8a834-133">无</span><span class="sxs-lookup"><span data-stu-id="8a834-133">None</span></span> |<span data-ttu-id="8a834-134">删除 calendar 对象。</span><span class="sxs-lookup"><span data-stu-id="8a834-134">Delete calendar object.</span></span> |
|[<span data-ttu-id="8a834-135">列出 calendarView</span><span class="sxs-lookup"><span data-stu-id="8a834-135">List calendarView</span></span>](../api/calendar-list-calendarview.md) |<span data-ttu-id="8a834-136">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-136">[event](event.md) collection</span></span>| <span data-ttu-id="8a834-137">从用户的主日历 `(../me/calendarview)` 或指定日历中，获取由时间范围定义的日历视图中的事件发生次数、异常和单个实例。</span><span class="sxs-lookup"><span data-stu-id="8a834-137">Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range, from the user's primary calendar `(../me/calendarview)` or from a specified calendar.</span></span>|
|[<span data-ttu-id="8a834-138">列出事件</span><span class="sxs-lookup"><span data-stu-id="8a834-138">List events</span></span>](../api/calendar-list-events.md) |<span data-ttu-id="8a834-139">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-139">[event](event.md) collection</span></span>| <span data-ttu-id="8a834-p107">检索日历中的事件列表。该列表包含单实例会议和系列主控事件。</span><span class="sxs-lookup"><span data-stu-id="8a834-p107">Retrieve a list of events in a calendar.  The list contains single instance meetings and series masters.</span></span>|
|[<span data-ttu-id="8a834-142">创建事件</span><span class="sxs-lookup"><span data-stu-id="8a834-142">Create event</span></span>](../api/calendar-post-events.md) |[<span data-ttu-id="8a834-143">event</span><span class="sxs-lookup"><span data-stu-id="8a834-143">event</span></span>](event.md)| <span data-ttu-id="8a834-144">在默认或指定日历中创建新事件。</span><span class="sxs-lookup"><span data-stu-id="8a834-144">Create a new event in the default or specified calendar.</span></span>|
|[<span data-ttu-id="8a834-145">getSchedule</span><span class="sxs-lookup"><span data-stu-id="8a834-145">getSchedule</span></span>](../api/calendar-getschedule.md) |<span data-ttu-id="8a834-146">[scheduleInformation](scheduleinformation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-146">[scheduleInformation](scheduleinformation.md) collection</span></span>|<span data-ttu-id="8a834-147">获取用户、通讯组列表或资源在指定时间段内的忙/闲状态信息。</span><span class="sxs-lookup"><span data-stu-id="8a834-147">Get the free/busy availability information for a collection of users, distributions lists, or resources, for a specified time period.</span></span> |
|[<span data-ttu-id="8a834-148">findMeetingTimes</span><span class="sxs-lookup"><span data-stu-id="8a834-148">findMeetingTimes</span></span>](../api/user-findmeetingtimes.md) |[<span data-ttu-id="8a834-149">meetingTimeSuggestionsResult</span><span class="sxs-lookup"><span data-stu-id="8a834-149">meetingTimeSuggestionsResult</span></span>](meetingtimesuggestionsresult.md) |<span data-ttu-id="8a834-150">根据组织者和与会者忙/闲状态以及时间或地点约束，建议会议时间和地点。</span><span class="sxs-lookup"><span data-stu-id="8a834-150">Suggest meeting times and locations based on organizer and attendee availability, and time or location constraints.</span></span> |
|[<span data-ttu-id="8a834-151">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="8a834-151">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="8a834-152">日历</span><span class="sxs-lookup"><span data-stu-id="8a834-152">calendar</span></span>](calendar.md)  |<span data-ttu-id="8a834-153">在新建或现有日历中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8a834-153">Create one or more single-value extended properties in a new or existing calendar.</span></span>   |
|[<span data-ttu-id="8a834-154">获取包含单值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="8a834-154">Get calendar with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8a834-155">日历</span><span class="sxs-lookup"><span data-stu-id="8a834-155">calendar</span></span>](calendar.md) | <span data-ttu-id="8a834-156">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-156">Get calendars that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="8a834-157">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="8a834-157">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="8a834-158">日历</span><span class="sxs-lookup"><span data-stu-id="8a834-158">calendar</span></span>](calendar.md) | <span data-ttu-id="8a834-159">在新建或现有的日历中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="8a834-159">Create one or more multi-value extended properties in a new or existing calendar.</span></span>  |
|[<span data-ttu-id="8a834-160">获取包含多值扩展属性的日历</span><span class="sxs-lookup"><span data-stu-id="8a834-160">Get calendar with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="8a834-161">日历</span><span class="sxs-lookup"><span data-stu-id="8a834-161">calendar</span></span>](calendar.md) | <span data-ttu-id="8a834-162">使用 `$expand` 获取包含一个多值扩展属性的日历。</span><span class="sxs-lookup"><span data-stu-id="8a834-162">Get a calendar that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="8a834-163">属性</span><span class="sxs-lookup"><span data-stu-id="8a834-163">Properties</span></span>
| <span data-ttu-id="8a834-164">属性</span><span class="sxs-lookup"><span data-stu-id="8a834-164">Property</span></span>     | <span data-ttu-id="8a834-165">类型</span><span class="sxs-lookup"><span data-stu-id="8a834-165">Type</span></span>   |<span data-ttu-id="8a834-166">Description</span><span class="sxs-lookup"><span data-stu-id="8a834-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a834-167">allowedOnlineMeetingProviders</span><span class="sxs-lookup"><span data-stu-id="8a834-167">allowedOnlineMeetingProviders</span></span>|<span data-ttu-id="8a834-168">OnlineMeetingProviderType 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-168">onlineMeetingProviderType collection</span></span>| <span data-ttu-id="8a834-169">表示此日历中可用于创建联机会议的联机会议服务提供商。</span><span class="sxs-lookup"><span data-stu-id="8a834-169">Represent the online meeting service providers that can be used to create online meetings in this calendar.</span></span> <span data-ttu-id="8a834-170">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="8a834-170">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="8a834-171">canEdit</span><span class="sxs-lookup"><span data-stu-id="8a834-171">canEdit</span></span> |<span data-ttu-id="8a834-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-172">Boolean</span></span> |<span data-ttu-id="8a834-173">`true` 如果用户可以写入日历，则 `false` 更改。</span><span class="sxs-lookup"><span data-stu-id="8a834-173">`true` if the user can write to the calendar, `false` otherwise.</span></span> <span data-ttu-id="8a834-174">此属性 `true` 日历的用户所使用。</span><span class="sxs-lookup"><span data-stu-id="8a834-174">This property is `true` for the user who created the calendar.</span></span> <span data-ttu-id="8a834-175">此属性也 `true` 已共享日历并授予写入访问权限的用户使用。</span><span class="sxs-lookup"><span data-stu-id="8a834-175">This property is also `true` for a user who has been shared a calendar and granted write access.</span></span> |
|<span data-ttu-id="8a834-176">canShare</span><span class="sxs-lookup"><span data-stu-id="8a834-176">canShare</span></span> |<span data-ttu-id="8a834-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-177">Boolean</span></span> |<span data-ttu-id="8a834-178">`true` 如果用户有共享日历的权限，则 `false` 更改。</span><span class="sxs-lookup"><span data-stu-id="8a834-178">`true` if the user has the permission to share the calendar, `false` otherwise.</span></span> <span data-ttu-id="8a834-179">只有创建日历的用户才可以进行共享。</span><span class="sxs-lookup"><span data-stu-id="8a834-179">Only the user who created the calendar can share it.</span></span> |
|<span data-ttu-id="8a834-180">canViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="8a834-180">canViewPrivateItems</span></span> |<span data-ttu-id="8a834-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-181">Boolean</span></span> |<span data-ttu-id="8a834-182">`true` 如果用户可以阅读标记为私密的日历项目，则 `false` 更改。</span><span class="sxs-lookup"><span data-stu-id="8a834-182">`true` if the user can read calendar items that have been marked private, `false` otherwise.</span></span> |
|<span data-ttu-id="8a834-183">changeKey</span><span class="sxs-lookup"><span data-stu-id="8a834-183">changeKey</span></span>|<span data-ttu-id="8a834-184">字符串</span><span class="sxs-lookup"><span data-stu-id="8a834-184">String</span></span>|<span data-ttu-id="8a834-p111">标识 calendar 对象的版本。每次日历更改时，changeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。只读。</span><span class="sxs-lookup"><span data-stu-id="8a834-p111">Identifies the version of the calendar object. Every time the calendar is changed, changeKey changes as well. This allows Exchange to apply changes to the correct version of the object. Read-only.</span></span>|
|<span data-ttu-id="8a834-189">颜色</span><span class="sxs-lookup"><span data-stu-id="8a834-189">color</span></span>|<span data-ttu-id="8a834-190">calendarColor</span><span class="sxs-lookup"><span data-stu-id="8a834-190">calendarColor</span></span>|<span data-ttu-id="8a834-191">在 UI 中指定将该日历与其他日历区分开来的颜色主题。</span><span class="sxs-lookup"><span data-stu-id="8a834-191">Specifies the color theme to distinguish the calendar from other calendars in a UI.</span></span> <span data-ttu-id="8a834-192">属性值为： `auto`、 `lightBlue`、 `lightGreen`、 `lightOrange`、 `lightGray`、 `lightYellow`、 `lightTeal`、 `lightPink`、 `lightBrown`、 `lightRed`、 `maxColor`。</span><span class="sxs-lookup"><span data-stu-id="8a834-192">The property values are: `auto`, `lightBlue`, `lightGreen`, `lightOrange`, `lightGray`, `lightYellow`, `lightTeal`, `lightPink`, `lightBrown`, `lightRed`, `maxColor`.</span></span>|
|<span data-ttu-id="8a834-193">defaultOnlineMeetingProvider</span><span class="sxs-lookup"><span data-stu-id="8a834-193">defaultOnlineMeetingProvider</span></span>|<span data-ttu-id="8a834-194">onlineMeetingProviderType</span><span class="sxs-lookup"><span data-stu-id="8a834-194">onlineMeetingProviderType</span></span>|<span data-ttu-id="8a834-195">从此日历发送的会议的默认联机会议提供商。</span><span class="sxs-lookup"><span data-stu-id="8a834-195">The default online meeting provider for meetings sent from this calendar.</span></span> <span data-ttu-id="8a834-196">可取值为：`unknown`、`skypeForBusiness`、`skypeForConsumer`、`teamsForBusiness`。</span><span class="sxs-lookup"><span data-stu-id="8a834-196">Possible values are: `unknown`, `skypeForBusiness`, `skypeForConsumer`, `teamsForBusiness`.</span></span>|
|<span data-ttu-id="8a834-197">hexColor</span><span class="sxs-lookup"><span data-stu-id="8a834-197">hexColor</span></span> |<span data-ttu-id="8a834-198">String</span><span class="sxs-lookup"><span data-stu-id="8a834-198">String</span></span> |<span data-ttu-id="8a834-199">日历颜色，以三个十六进制值的六进制值（每个值从 00 到 FF）表示，表示 RGB 颜色空间内颜色的红色、绿色或蓝色组成部分。</span><span class="sxs-lookup"><span data-stu-id="8a834-199">The calendar color, expressed in a hex color code of three hexadecimal values, each ranging from 00 to FF and representing the red, green, or blue components of the color in the RGB color space.</span></span> <span data-ttu-id="8a834-200">若用户从未明确设置日历的颜色，则此属性为空。</span><span class="sxs-lookup"><span data-stu-id="8a834-200">If the user has never explicitly set a color for the calendar, this property is empty.</span></span> <span data-ttu-id="8a834-201">只读。</span><span class="sxs-lookup"><span data-stu-id="8a834-201">Read-only.</span></span>|
|<span data-ttu-id="8a834-202">id</span><span class="sxs-lookup"><span data-stu-id="8a834-202">id</span></span>|<span data-ttu-id="8a834-203">String</span><span class="sxs-lookup"><span data-stu-id="8a834-203">String</span></span>|<span data-ttu-id="8a834-p115">日历的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="8a834-p115">The calendar's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="8a834-206">isDefaultCalendar</span><span class="sxs-lookup"><span data-stu-id="8a834-206">isDefaultCalendar</span></span>|<span data-ttu-id="8a834-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-207">Boolean</span></span>|<span data-ttu-id="8a834-208">`true` 如果这是默认情况下创建新事件的默认日历，则 `false` 更改。</span><span class="sxs-lookup"><span data-stu-id="8a834-208">`true` if this is the default calendar where new events are created by default, `false` otherwise.</span></span>|
|<span data-ttu-id="8a834-209">isRemovable</span><span class="sxs-lookup"><span data-stu-id="8a834-209">isRemovable</span></span>|<span data-ttu-id="8a834-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-210">Boolean</span></span>| <span data-ttu-id="8a834-211">表示是否可以从用户邮箱删除此用户日志。</span><span class="sxs-lookup"><span data-stu-id="8a834-211">Indicates whether this user calendar can be deleted from the user mailbox.</span></span>|
|<span data-ttu-id="8a834-212">isTallyingResponses</span><span class="sxs-lookup"><span data-stu-id="8a834-212">isTallyingResponses</span></span>|<span data-ttu-id="8a834-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="8a834-213">Boolean</span></span>|<span data-ttu-id="8a834-214">表示此用户日历是否支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="8a834-214">Indicates whether this user calendar supports tracking of meeting responses.</span></span> <span data-ttu-id="8a834-215">仅从用户的主日志发送的会议邀请支持会议响应跟踪。</span><span class="sxs-lookup"><span data-stu-id="8a834-215">Only meeting invites sent from users' primary calendars support tracking of meeting responses.</span></span>|
|<span data-ttu-id="8a834-216">name</span><span class="sxs-lookup"><span data-stu-id="8a834-216">name</span></span>|<span data-ttu-id="8a834-217">String</span><span class="sxs-lookup"><span data-stu-id="8a834-217">String</span></span>|<span data-ttu-id="8a834-218">日历名称。</span><span class="sxs-lookup"><span data-stu-id="8a834-218">The calendar name.</span></span>|
|<span data-ttu-id="8a834-219">owner</span><span class="sxs-lookup"><span data-stu-id="8a834-219">owner</span></span> |[<span data-ttu-id="8a834-220">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8a834-220">emailAddress</span></span>](emailaddress.md) | <span data-ttu-id="8a834-p117">如果设置，则表示创建或添加日历的用户。对于用户创建或添加的日历，将 **owner** 属性设置为用户。对于与用户共享的日历，将 **owner** 属性设置为与此用户共享该日历的人员。</span><span class="sxs-lookup"><span data-stu-id="8a834-p117">If set, this represents the user who created or added the calendar. For a calendar that the user created or added, the **owner** property is set to the user. For a calendar shared with the user, the **owner** property is set to the person who shared that calendar with the user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8a834-224">关系</span><span class="sxs-lookup"><span data-stu-id="8a834-224">Relationships</span></span>
| <span data-ttu-id="8a834-225">关系</span><span class="sxs-lookup"><span data-stu-id="8a834-225">Relationship</span></span> | <span data-ttu-id="8a834-226">类型</span><span class="sxs-lookup"><span data-stu-id="8a834-226">Type</span></span>   |<span data-ttu-id="8a834-227">Description</span><span class="sxs-lookup"><span data-stu-id="8a834-227">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8a834-228">calendarPermissions</span><span class="sxs-lookup"><span data-stu-id="8a834-228">calendarPermissions</span></span>|<span data-ttu-id="8a834-229">[calendarPermission](calendarpermission.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-229">[calendarPermission](calendarpermission.md) collection</span></span>| <span data-ttu-id="8a834-230">共享日历的用户的权限。</span><span class="sxs-lookup"><span data-stu-id="8a834-230">The permissions of the users with whom the calendar is shared.</span></span>|
|<span data-ttu-id="8a834-231">calendarView</span><span class="sxs-lookup"><span data-stu-id="8a834-231">calendarView</span></span>|<span data-ttu-id="8a834-232">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-232">[Event](event.md) collection</span></span>|<span data-ttu-id="8a834-p118">日历的日历视图。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="8a834-p118">The calendar view for the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="8a834-236">events</span><span class="sxs-lookup"><span data-stu-id="8a834-236">events</span></span>|<span data-ttu-id="8a834-237">[事件](event.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-237">[Event](event.md) collection</span></span>|<span data-ttu-id="8a834-p119">日历中的事件。导航属性。只读。</span><span class="sxs-lookup"><span data-stu-id="8a834-p119">The events in the calendar. Navigation property. Read-only.</span></span>|
|<span data-ttu-id="8a834-241">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8a834-241">multiValueExtendedProperties</span></span>|<span data-ttu-id="8a834-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8a834-242">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="8a834-p120">为日历定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a834-p120">The collection of multi-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|
|<span data-ttu-id="8a834-246">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="8a834-246">singleValueExtendedProperties</span></span>|<span data-ttu-id="8a834-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="8a834-247">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="8a834-p121">为日历定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="8a834-p121">The collection of single-value extended properties defined for the calendar. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8a834-251">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8a834-251">JSON representation</span></span>

<span data-ttu-id="8a834-252">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8a834-252">Here is a JSON representation of the resource</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [
    "calendarView",
    "events",
    "multiValueExtendedProperties",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.calendar",
  "@odata.annotations": [
    {
      "property": "calendarView",
      "capabilities": {
        "changeTracking": true,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "navigability": "single",
        "searchable": false,
        "updatable": false
      }
    },
    {
      "property": "events",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "navigability": "single",
        "searchable": false
      }
    }
  ]
}-->

```json
{
  "allowedOnlineMeetingProviders": ["string"],
  "canEdit": "boolean",
  "canShare": "boolean",
  "canViewPrivateItems": "boolean",
  "changeKey": "string",
  "color": "String",
  "defaultOnlineMeetingProvider": "string",
  "hexColor": "String",
  "id": "string (identifier)",
  "isDefaultCalendar": "boolean",
  "isRemovable": "boolean",
  "isTallyingResponses": "boolean",
  "name": "string",
  "owner": {"@odata.type": "microsoft.graph.emailAddress"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "calendar resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

