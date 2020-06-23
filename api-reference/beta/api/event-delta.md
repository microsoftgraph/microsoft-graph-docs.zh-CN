---
title: 'event: delta'
description: 获取 **calendarView**（事件范围）中已添加、删除或更新的事件集。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 61ca6937622eadc16aafc1e8c97f38e1fd0db8a2
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845321"
---
# <a name="event-delta"></a><span data-ttu-id="e8516-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="e8516-103">event: delta</span></span>

<span data-ttu-id="e8516-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e8516-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e8516-105">获取一组在一个或多个日历中添加、删除或更新的[事件](../resources/event.md)资源。</span><span class="sxs-lookup"><span data-stu-id="e8516-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="e8516-106">可以在邮箱的所有日历或特定日历中的事件中或在**calendarView**的事件集合（由日历的开始日期和结束日期定义的事件范围）中获取这些增量更改的特定类型。</span><span class="sxs-lookup"><span data-stu-id="e8516-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="e8516-107">日历可以是用户的默认日历或其他指定的日历。</span><span class="sxs-lookup"><span data-stu-id="e8516-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="e8516-108">在**calendarView**中获取增量更改的情况下，日历也可以是组日历。</span><span class="sxs-lookup"><span data-stu-id="e8516-108">In the case of getting incremental changes on **calendarView**, the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="e8516-109">**Delta**函数调用类似于 `GET /events` 或 `GET /calendarview` 请求指定的日历，不同之处在于，通过在一个或多个调用中正确应用[状态令牌](/graph/delta-query-overview#state-tokens)，可以在该日历中查询事件的增量更改。</span><span class="sxs-lookup"><span data-stu-id="e8516-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="e8516-110">这样，您就可以在指定的日历中维护和同步事件的本地存储，而无需每次从服务器提取该日历的所有事件。</span><span class="sxs-lookup"><span data-stu-id="e8516-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="e8516-111">下表列出了事件中的**delta**函数和日历中的**calendarView**上的**delta**函数之间的差异。</span><span class="sxs-lookup"><span data-stu-id="e8516-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="e8516-112">事件的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-112">Delta function on events</span></span>  | <span data-ttu-id="e8516-113">CalendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="e8516-114">获取不受开始和结束日期范围限制的日历中的所有事件的增量更改。</span><span class="sxs-lookup"><span data-stu-id="e8516-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="e8516-115">此外，还可以在开始时间之后的日历中获取事件的增量更改，该日历在日期/时间开始或之后。</span><span class="sxs-lookup"><span data-stu-id="e8516-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="e8516-116">获取**calendarView**的开始和结束日期/时间内的事件的增量更改。</span><span class="sxs-lookup"><span data-stu-id="e8516-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="e8516-117">出于性能原因，仅返回一组有限的**事件**属性。</span><span class="sxs-lookup"><span data-stu-id="e8516-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="e8516-118">随后用于 `GET /events/{id}` 扩展任何事件的客户端。</span><span class="sxs-lookup"><span data-stu-id="e8516-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="e8516-119">服务器端扩展返回一组更完整的**事件**属性。</span><span class="sxs-lookup"><span data-stu-id="e8516-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="e8516-120">响应包括单个实例和定期系列主机。</span><span class="sxs-lookup"><span data-stu-id="e8516-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="e8516-121">响应包括单个实例以及定期系列的匹配项和例外。</span><span class="sxs-lookup"><span data-stu-id="e8516-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="e8516-122">适用于用户日历中的事件，但不是组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="e8516-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="e8516-123">适用于用户和组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="e8516-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="e8516-124">当前仅在 beta 版本中可用。</span><span class="sxs-lookup"><span data-stu-id="e8516-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="e8516-125">在 v1.0 和 beta 版本中可用。</span><span class="sxs-lookup"><span data-stu-id="e8516-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="e8516-126">Permissions</span><span class="sxs-lookup"><span data-stu-id="e8516-126">Permissions</span></span>
<span data-ttu-id="e8516-127">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e8516-127">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e8516-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8516-128">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8516-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8516-129">Permission type</span></span>      | <span data-ttu-id="e8516-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8516-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8516-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8516-131">Delegated (work or school account)</span></span> | <span data-ttu-id="e8516-132">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8516-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e8516-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8516-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e8516-134">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8516-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="e8516-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8516-135">Application</span></span> | <span data-ttu-id="e8516-136">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e8516-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e8516-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8516-137">HTTP request</span></span>

<span data-ttu-id="e8516-138">此部分显示初始**delta**函数调用的 HTTP 请求语法，以启动完全同步，以检索指定日历视图或日历视图中的所有事件。</span><span class="sxs-lookup"><span data-stu-id="e8516-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="e8516-139">此语法不包含任何[状态令牌](/graph/delta-query-overview#state-tokens)。</span><span class="sxs-lookup"><span data-stu-id="e8516-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="e8516-140">在或成功响应中返回的查询 URL `nextLink` `deltaLink` 包括状态令牌。</span><span class="sxs-lookup"><span data-stu-id="e8516-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="e8516-141">对于任何后续的**delta**函数调用，使用 `nextLink` 或在其前面的查询 URL `deltaLink` 。</span><span class="sxs-lookup"><span data-stu-id="e8516-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="e8516-142">用户日历中的事件的 Delta 函数（预览）</span><span class="sxs-lookup"><span data-stu-id="e8516-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="e8516-143">在指定的用户日历中，对在特定日期/时间开始或之后开始的所有事件或事件应用**delta**函数：</span><span class="sxs-lookup"><span data-stu-id="e8516-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="e8516-144">若要获取_用户邮箱中_的所有事件或在指定的日期/时间之后或之后开始的事件的增量更改，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="e8516-145">若要获取_用户的默认日历中_的所有事件或在指定的日期/时间之后或之后开始的事件的增量更改，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="e8516-146">若要获取对_指定的用户日历中_的所有事件或在指定的日期/时间之后开始或之后的事件的增量更改，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="e8516-147">若要获取_默认日历组的指定日历中_的所有事件或在指定的日期/时间之后或之后开始或之后的事件的增量更改，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-147">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified calendar of the default calendar group_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroup/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta 

  GET /me/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="e8516-148">若要获取增量更改_指定的日历组和日历中_的所有事件或在指定的日期/时间之后或之后开始的事件，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-148">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendargroups/{id}/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta 

  GET /me/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

<!-- Add back and fix html when group calendars are supported

### Delta function on events in a group calendar (preview)
* To get incremental changes of all the events, or of events starting on or after the specified date/time _in a group calendar_:
  !-- { "blockType": "ignored" } --
  ```http
  GET /groups/{id}/events/delta
  GET /groups/{id}/calendar/events/delta

  GET /groups/{id}/events/delta?startDateTime={start_datetime}
  GET /groups/{id}/calendar/events/delta?startDateTime={start_datetime}
  ```

  -->

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="e8516-149">用户日历中的 calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-149">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="e8516-150">在指定的用户日历中，对由开始和结束日期/时间分隔的一系列事件应用**delta**函数：</span><span class="sxs-lookup"><span data-stu-id="e8516-150">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="e8516-151">在_用户的默认日历_的 "日历" 视图中获取增量更改：</span><span class="sxs-lookup"><span data-stu-id="e8516-151">To get incremental changes in a calendar view of _the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="e8516-152">若要获取_指定用户日历_的日历视图中的增量更改，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-152">To get incremental changes in a calendar view of _the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="e8516-153">组日历中的 calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-153">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="e8516-154">若要在_组日历_的日历视图中获取增量更改，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="e8516-154">To get incremental changes in a calendar view of _a group's calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="e8516-155">查询参数</span><span class="sxs-lookup"><span data-stu-id="e8516-155">Query parameters</span></span>

<span data-ttu-id="e8516-156">跟踪更改会产生一个或多个**delta**函数调用的往返。</span><span class="sxs-lookup"><span data-stu-id="e8516-156">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="e8516-157">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="e8516-157">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="e8516-158">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="e8516-158">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="e8516-159">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="e8516-159">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="e8516-160">在后续请求中，只需复制并 `nextLink` 应用 `deltaLink` 上一个响应中的或 url，因为该 URL 已包含已编码的所需参数。</span><span class="sxs-lookup"><span data-stu-id="e8516-160">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="e8516-161">查询参数</span><span class="sxs-lookup"><span data-stu-id="e8516-161">Query parameter</span></span>      | <span data-ttu-id="e8516-162">类型</span><span class="sxs-lookup"><span data-stu-id="e8516-162">Type</span></span>   |<span data-ttu-id="e8516-163">说明</span><span class="sxs-lookup"><span data-stu-id="e8516-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e8516-164">startDateTime</span><span class="sxs-lookup"><span data-stu-id="e8516-164">startDateTime</span></span>|<span data-ttu-id="e8516-165">String</span><span class="sxs-lookup"><span data-stu-id="e8516-165">String</span></span>|<span data-ttu-id="e8516-166">The start date and time of the time range, represented in ISO 8601 format.</span><span class="sxs-lookup"><span data-stu-id="e8516-166">The start date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="e8516-167">For example, "2019-11-08T19:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="e8516-167">For example, "2019-11-08T19:00:00-08:00".</span></span> <br><span data-ttu-id="e8516-168">时区在参数值的 "时区偏移" 部分中指定，如果存在，则不受 `Prefer: outlook.timezone` 标头的影响。</span><span class="sxs-lookup"><span data-stu-id="e8516-168">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="e8516-169">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="e8516-169">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="e8516-170">对于日历中事件的**delta**是可选的。</span><span class="sxs-lookup"><span data-stu-id="e8516-170">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="e8516-171">对于**calendarView**上的**delta**是必需的。</span><span class="sxs-lookup"><span data-stu-id="e8516-171">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="e8516-172">endDateTime</span><span class="sxs-lookup"><span data-stu-id="e8516-172">endDateTime</span></span>|<span data-ttu-id="e8516-173">String</span><span class="sxs-lookup"><span data-stu-id="e8516-173">String</span></span>|<span data-ttu-id="e8516-174">The end date and time of the time range, represented in ISO 8601 format.</span><span class="sxs-lookup"><span data-stu-id="e8516-174">The end date and time of the time range, represented in ISO 8601 format.</span></span> <span data-ttu-id="e8516-175">For example, "2019-11-08T20:00:00-08:00".</span><span class="sxs-lookup"><span data-stu-id="e8516-175">For example, "2019-11-08T20:00:00-08:00".</span></span> <br><span data-ttu-id="e8516-176">时区在参数值的 "时区偏移" 部分中指定，如果存在，则不受 `Prefer: outlook.timezone` 标头的影响。</span><span class="sxs-lookup"><span data-stu-id="e8516-176">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="e8516-177">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="e8516-177">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="e8516-178">日历中的事件_不支持_**增量**。</span><span class="sxs-lookup"><span data-stu-id="e8516-178">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="e8516-179">对于**calendarView**上的**delta**是必需的。</span><span class="sxs-lookup"><span data-stu-id="e8516-179">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="e8516-180">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="e8516-180">$deltatoken</span></span> | <span data-ttu-id="e8516-181">string</span><span class="sxs-lookup"><span data-stu-id="e8516-181">string</span></span> | <span data-ttu-id="e8516-182">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking.</span><span class="sxs-lookup"><span data-stu-id="e8516-182">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking.</span></span> <span data-ttu-id="e8516-183">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span><span class="sxs-lookup"><span data-stu-id="e8516-183">Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="e8516-184">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="e8516-184">$skiptoken</span></span> | <span data-ttu-id="e8516-185">string</span><span class="sxs-lookup"><span data-stu-id="e8516-185">string</span></span> | <span data-ttu-id="e8516-186">之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个日历视图中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="e8516-186">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="e8516-187">不支持 `$expand` 、 `$filter` 、、 `$orderby` `$select` 和 `$search` 。</span><span class="sxs-lookup"><span data-stu-id="e8516-187">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="e8516-188">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8516-188">Request headers</span></span>
| <span data-ttu-id="e8516-189">名称</span><span class="sxs-lookup"><span data-stu-id="e8516-189">Name</span></span>       | <span data-ttu-id="e8516-190">类型</span><span class="sxs-lookup"><span data-stu-id="e8516-190">Type</span></span> | <span data-ttu-id="e8516-191">Description</span><span class="sxs-lookup"><span data-stu-id="e8516-191">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="e8516-192">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8516-192">Authorization</span></span>  | <span data-ttu-id="e8516-193">字符串</span><span class="sxs-lookup"><span data-stu-id="e8516-193">string</span></span>  | <span data-ttu-id="e8516-194">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="e8516-194">Bearer {token}.</span></span> <span data-ttu-id="e8516-195">Required.</span><span class="sxs-lookup"><span data-stu-id="e8516-195">Required.</span></span> |
| <span data-ttu-id="e8516-196">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8516-196">Content-Type</span></span>  | <span data-ttu-id="e8516-197">字符串</span><span class="sxs-lookup"><span data-stu-id="e8516-197">string</span></span>  | <span data-ttu-id="e8516-198">application/json.</span><span class="sxs-lookup"><span data-stu-id="e8516-198">application/json.</span></span> <span data-ttu-id="e8516-199">Required.</span><span class="sxs-lookup"><span data-stu-id="e8516-199">Required.</span></span> |
| <span data-ttu-id="e8516-200">Prefer</span><span class="sxs-lookup"><span data-stu-id="e8516-200">Prefer</span></span> | <span data-ttu-id="e8516-201">string</span><span class="sxs-lookup"><span data-stu-id="e8516-201">string</span></span>  | <span data-ttu-id="e8516-202">odata.maxpagesize={x}.</span><span class="sxs-lookup"><span data-stu-id="e8516-202">odata.maxpagesize={x}.</span></span> <span data-ttu-id="e8516-203">Optional.</span><span class="sxs-lookup"><span data-stu-id="e8516-203">Optional.</span></span> |
| <span data-ttu-id="e8516-204">Prefer</span><span class="sxs-lookup"><span data-stu-id="e8516-204">Prefer</span></span> | <span data-ttu-id="e8516-205">string</span><span class="sxs-lookup"><span data-stu-id="e8516-205">string</span></span> | <span data-ttu-id="e8516-206">outlook. 时区 = {时区字符串}。</span><span class="sxs-lookup"><span data-stu-id="e8516-206">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="e8516-207">可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="e8516-207">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="e8516-208">响应</span><span class="sxs-lookup"><span data-stu-id="e8516-208">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="e8516-209">事件的 Delta 函数（预览）</span><span class="sxs-lookup"><span data-stu-id="e8516-209">Delta function on events (preview)</span></span>
<span data-ttu-id="e8516-210">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[event](../resources/event.md)集合。</span><span class="sxs-lookup"><span data-stu-id="e8516-210">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="e8516-211">由于性能原因，响应中的每个**事件**仅包含**id**、**类型**、**起始**和**结束**属性。</span><span class="sxs-lookup"><span data-stu-id="e8516-211">Each **event** in the response contains only the **id**, **type**, **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="e8516-212">随后使用将 `GET /events/{id}` 任何事件从响应中展开。</span><span class="sxs-lookup"><span data-stu-id="e8516-212">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="e8516-213">CalendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-213">Delta function on calendarView</span></span>
<span data-ttu-id="e8516-214">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[event](../resources/event.md)集合。</span><span class="sxs-lookup"><span data-stu-id="e8516-214">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="e8516-215">希望获取您通常从请求获取的所有属性 `GET /calendarview` 。</span><span class="sxs-lookup"><span data-stu-id="e8516-215">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="e8516-216">示例</span><span class="sxs-lookup"><span data-stu-id="e8516-216">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="e8516-217">示例1：日历中事件的 Delta 函数（预览）</span><span class="sxs-lookup"><span data-stu-id="e8516-217">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="e8516-218">请求</span><span class="sxs-lookup"><span data-stu-id="e8516-218">Request</span></span>
<span data-ttu-id="e8516-219">以下示例显示了用于获取登录用户的默认日历中的事件的初始同步请求，该事件发生在指定参数之前或之后 `startDateTime` 。</span><span class="sxs-lookup"><span data-stu-id="e8516-219">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="e8516-220">初始请求不包含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="e8516-220">The initial request does not include any state token.</span></span> 

<span data-ttu-id="e8516-221">请求使用 `Prefer: odata.maxpagesize` 标头将每个响应中的最大事件数限制为1。</span><span class="sxs-lookup"><span data-stu-id="e8516-221">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="e8516-222">在 `delta` 收到响应之前，使用返回的查询继续调用该函数 `@odata.nextLink` `@odata.deltaLink` 。</span><span class="sxs-lookup"><span data-stu-id="e8516-222">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="e8516-223">响应</span><span class="sxs-lookup"><span data-stu-id="e8516-223">Response</span></span>

<span data-ttu-id="e8516-224">如果请求成功，则响应包含一个状态令牌，该令牌是_skipToken_ （在_ \@ nextLink_响应头中）或_deltaToken_ （在_ \@ odata. deltaLink_响应头中）。</span><span class="sxs-lookup"><span data-stu-id="e8516-224">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="e8516-225">它们分别指示是否应继续进行循环，或者是否已完成对该轮的所有更改的获取。</span><span class="sxs-lookup"><span data-stu-id="e8516-225">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="e8516-226">下面的响应显示_ \@ nextLink_响应头中的_skipToken_ 。</span><span class="sxs-lookup"><span data-stu-id="e8516-226">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<!-- {
  "blockType": "response",
  "name": "event_delta_events",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendar/events/delta?$skiptoken=R0usmcdvmMu7jxWP8",
  "value": [
    { 
      "id": " AAMkADllMWMwNDkzLWJlY2EtNDIyOS1iZjAA=", 
      "type": "singleInstance", 
      "start": {  
             "DateTime": "2020-02-19T10:00:00.0000000",  
             "TimeZone": "UTC" 
         },  
       "end": {  
                "DateTime": "2020-02-19T11:00:00.0000000",  
                "TimeZone": "UTC"        
          }  
        } 
  ]
}
```


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="e8516-227">示例2： calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="e8516-227">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="e8516-228">请求</span><span class="sxs-lookup"><span data-stu-id="e8516-228">Request</span></span>

<span data-ttu-id="e8516-229">下面的示例显示了在**calendarView**指定的日期范围内，要获取已登录用户的指定日历中的事件的初始同步请求。</span><span class="sxs-lookup"><span data-stu-id="e8516-229">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="e8516-230">初始请求不包含任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="e8516-230">The initial request does not include any state token.</span></span> 

<span data-ttu-id="e8516-231">请求使用 `Prefer: odata.maxpagesize` 标头将每个响应中的最大事件数限制为2个。</span><span class="sxs-lookup"><span data-stu-id="e8516-231">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="e8516-232">使用返回的查询继续调用该 `delta` 函数 `@odata.nextLink` ，直到您获取该日历视图中的所有事件以及 `@odata.deltaLink` 响应中的。</span><span class="sxs-lookup"><span data-stu-id="e8516-232">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="e8516-233">HTTP</span><span class="sxs-lookup"><span data-stu-id="e8516-233">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="e8516-234">C#</span><span class="sxs-lookup"><span data-stu-id="e8516-234">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e8516-235">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e8516-235">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="e8516-236">响应</span><span class="sxs-lookup"><span data-stu-id="e8516-236">Response</span></span>

<span data-ttu-id="e8516-237">如果请求成功，则响应包含一个状态令牌，该令牌是_skipToken_ （在_ \@ nextLink_响应头中）或_deltaToken_ （在_ \@ odata. deltaLink_响应头中）。</span><span class="sxs-lookup"><span data-stu-id="e8516-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="e8516-238">它们分别指示是否应继续进行循环，或者是否已完成对该轮的所有更改的获取。</span><span class="sxs-lookup"><span data-stu-id="e8516-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="e8516-239">下面的响应显示_ \@ nextLink_响应头中的_skipToken_ 。</span><span class="sxs-lookup"><span data-stu-id="e8516-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="e8516-240">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e8516-240">Note: The response object shown here may be truncated for brevity.</span></span> 
<!-- {
  "blockType": "response",
  "name": "event_delta_calendarview",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(event)",
    "@odata.nextLink": "https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?$skiptoken=R0usmcdvmMu7jxWP8",
    "value": [
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTgw==\"",
            "createdDateTime": "2020-06-16T04:05:43.8668791Z",
            "lastModifiedDateTime": "2020-06-16T04:08:27.354268Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTgw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E00800000000F088B8B95843D601000000000000000010000000165CD5547CFC9545B6492B261750B48C",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": false,
            "hasAttachments": false,
            "subject": "Summer party",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1QAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1QAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-02T20:00:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-02T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.event",
            "@odata.etag": "W/\"Jdsb3FEkPk2qoUHCdliYowACwixTfw==\"",
            "createdDateTime": "2020-06-16T04:06:18.386713Z",
            "lastModifiedDateTime": "2020-06-16T04:08:19.5694048Z",
            "changeKey": "Jdsb3FEkPk2qoUHCdliYowACwixTfw==",
            "categories": [],
            "transactionId": null,
            "originalStartTimeZone": "Pacific Standard Time",
            "originalEndTimeZone": "Pacific Standard Time",
            "uid": "040000008200E00074C5B7101A82E0080000000060074BC55843D6010000000000000000100000002D33A89F36B10D43A12FD990B62858B2",
            "reminderMinutesBeforeStart": 15,
            "isReminderOn": true,
            "hasAttachments": false,
            "subject": "Summer party part 2",
            "bodyPreview": "",
            "importance": "normal",
            "sensitivity": "normal",
            "isAllDay": false,
            "isCancelled": false,
            "isOrganizer": true,
            "IsRoomRequested": false,
            "AutoRoomBookingStatus": "None",
            "responseRequested": true,
            "seriesMasterId": null,
            "showAs": "busy",
            "type": "singleInstance",
            "webLink": "https://outlook.office365.com/owa/?itemid=AAMkADI5MAAKkeE1RAAA%3D&exvsurl=1&path=/calendar/item",
            "onlineMeetingUrl": null,
            "isOnlineMeeting": false,
            "onlineMeetingProvider": "unknown",
            "allowNewTimeProposals": true,
            "OccurrenceId": null,
            "isDraft": false,
            "recurrence": null,
            "AutoRoomBookingOptions": null,
            "onlineMeeting": null,
            "id": "AAMkADI5MAAKkeE1RAAA=",
            "responseStatus": {
                "response": "none",
                "time": "0001-01-01T00:00:00Z"
            },
            "body": {
                "contentType": "html",
                "content": "<html>\r\n<head></head>\r\n<body lang=\"EN-US\" link=\"#0563C1\" vlink=\"#954F72\" style=\"\">\r\n<div class=\"WordSection1\">\r\n<p class=\"MsoNormal\">&nbsp;</p>\r\n</div>\r\n</body>\r\n</html>\r\n"
            },
            "start": {
                "dateTime": "2020-06-04T19:30:00.0000000",
                "timeZone": "UTC"
            },
            "end": {
                "dateTime": "2020-06-04T22:30:00.0000000",
                "timeZone": "UTC"
            },
            "location": {
                "displayName": "",
                "locationType": "default",
                "uniqueIdType": "unknown",
                "address": {
                    "type": "unknown"
                },
                "coordinates": {}
            },
            "locations": [],
            "attendees": [
                {
                    "type": "required",
                    "status": {
                        "response": "none",
                        "time": "0001-01-01T00:00:00Z"
                    },
                    "emailAddress": {
                        "name": "Samantha Booth",
                        "address": "samanthab@contoso.onmicrosoft.com"
                    }
                }
            ],
            "organizer": {
                "emailAddress": {
                    "name": "Samantha Booth",
                    "address": "samanthab@contoso.onmicrosoft.com"
                }
            }
        }
    ]
}
```

### <a name="see-also"></a><span data-ttu-id="e8516-241">另请参阅</span><span class="sxs-lookup"><span data-stu-id="e8516-241">See also</span></span>

- [<span data-ttu-id="e8516-242">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="e8516-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="e8516-243">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="e8516-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "event: delta",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
