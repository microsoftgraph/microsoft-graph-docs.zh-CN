---
title: 'event: delta'
description: 获取 **calendarView**（事件范围）中已添加、删除或更新的事件集。
localization_priority: Normal
author: harini84
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: efa0768fbb8cae441afc3d1fd48baa2e2a3567da
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436244"
---
# <a name="event-delta"></a><span data-ttu-id="2843a-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="2843a-103">event: delta</span></span>

<span data-ttu-id="2843a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2843a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2843a-105">获取一 [组](../resources/event.md) 已在一个或多个日历中添加、删除或更新的事件资源。</span><span class="sxs-lookup"><span data-stu-id="2843a-105">Get a set of [event](../resources/event.md) resources that have been added, deleted, or updated in one or more calendars.</span></span> 

<span data-ttu-id="2843a-106">可以在邮箱的所有日历或特定日历中的事件或日历 **的日历视图** (事件范围（由日历的开始日期和结束日期) ）的事件集中获取这些增量更改的特定类型的更改。</span><span class="sxs-lookup"><span data-stu-id="2843a-106">You can get specific types of these incremental changes in the events in all the calendars of a mailbox or in a specific calendar, or in an event collection of a **calendarView** (range of events defined by start and end dates) of a calendar.</span></span> <span data-ttu-id="2843a-107">日历可以是默认日历或用户的其他一些指定日历。</span><span class="sxs-lookup"><span data-stu-id="2843a-107">The calendar can be the default calendar or some other specified calendar of the user's.</span></span> <span data-ttu-id="2843a-108">在 **calendarView** 上获取增量更改的情况下，日历也可以是组日历。</span><span class="sxs-lookup"><span data-stu-id="2843a-108">In the case of getting incremental changes on **calendarView**, the calendar can be a group calendar as well.</span></span>

<span data-ttu-id="2843a-109">**delta** 函数调用类似于指定日历的或请求，只不过通过在这些调用中的一个或多个调用中正确应用状态令牌，可以查询该日历中事件的增量更改。 `GET /events` `GET /calendarview` [](/graph/delta-query-overview#state-tokens)</span><span class="sxs-lookup"><span data-stu-id="2843a-109">A **delta** function call is similar to a `GET /events` or `GET /calendarview` request for the specified calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview#state-tokens) in one or more of these calls, you can query for incremental changes of events in that calender.</span></span> <span data-ttu-id="2843a-110">这允许您维护和同步指定日历中事件的本地存储，而无需每次从服务器提取该日历的所有事件。</span><span class="sxs-lookup"><span data-stu-id="2843a-110">This allows you to maintain and synchronize a local store of events in the specified calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

<span data-ttu-id="2843a-111">下表列出了事件上的 **delta** 函数与日历中 **calendarView** 上的 **delta** 函数之间的差异。</span><span class="sxs-lookup"><span data-stu-id="2843a-111">The following table lists the differences between the **delta** function on events and the **delta** function on a **calendarView** in a calendar.</span></span>

| <span data-ttu-id="2843a-112">事件上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-112">Delta function on events</span></span>  | <span data-ttu-id="2843a-113">calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-113">Delta function on calendarView</span></span>  |
|:--------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2843a-114">获取日历中不受开始日期和结束日期范围限制的所有事件的增量更改。</span><span class="sxs-lookup"><span data-stu-id="2843a-114">Gets incremental changes of all the events in a calendar not bounded by a start and end date range.</span></span> <span data-ttu-id="2843a-115">或者，你可以从该日期/时间或之后开始，获取受开始时间限制的日历中事件的增量更改。</span><span class="sxs-lookup"><span data-stu-id="2843a-115">Alternatively, you can get incremental changes of the events in a calendar bounded by a start time, starting on or after that date/time.</span></span> | <span data-ttu-id="2843a-116">获取日历视图 的开始日期和结束日期/时间内事件的 **增量更改**。</span><span class="sxs-lookup"><span data-stu-id="2843a-116">Gets incremental changes of events within the start and end date/time of the **calendarView**.</span></span> |
| <span data-ttu-id="2843a-117">出于性能原因，仅 **返回一组** 有限的事件属性。</span><span class="sxs-lookup"><span data-stu-id="2843a-117">Returns only a limited set of **event** properties for performance reasons.</span></span> <span data-ttu-id="2843a-118">随后用于扩展 `GET /events/{id}` 任何事件的客户端。</span><span class="sxs-lookup"><span data-stu-id="2843a-118">Client to subsequently use `GET /events/{id}` to expand any events.</span></span> | <span data-ttu-id="2843a-119">服务器端扩展返回一组更 **完整的事件** 属性。</span><span class="sxs-lookup"><span data-stu-id="2843a-119">Server-side expansion returns a fuller set of **event** properties.</span></span> |
| <span data-ttu-id="2843a-120">响应包括单个实例和定期系列母版。</span><span class="sxs-lookup"><span data-stu-id="2843a-120">Response includes single instances and recurring series master.</span></span> | <span data-ttu-id="2843a-121">响应包括单个实例，以及定期系列的发生和例外。</span><span class="sxs-lookup"><span data-stu-id="2843a-121">Response includes single instances, and occurrences and exceptions of recurring series.</span></span> |
| <span data-ttu-id="2843a-122">适用于用户日历中的事件，但不应用于组日历。</span><span class="sxs-lookup"><span data-stu-id="2843a-122">Applies to events in user calendars but not group calendars.</span></span> | <span data-ttu-id="2843a-123">适用于用户和组日历中的事件。</span><span class="sxs-lookup"><span data-stu-id="2843a-123">Applies to events in user and group calendars.</span></span> |
| <span data-ttu-id="2843a-124">当前仅在 beta 版本中可用。</span><span class="sxs-lookup"><span data-stu-id="2843a-124">Currently available only in the beta version.</span></span> | <span data-ttu-id="2843a-125">在 v1.0 和 beta 版本中可用。</span><span class="sxs-lookup"><span data-stu-id="2843a-125">Available in the v1.0 and beta versions.</span></span> |

## <a name="permissions"></a><span data-ttu-id="2843a-126">Permissions</span><span class="sxs-lookup"><span data-stu-id="2843a-126">Permissions</span></span>
<span data-ttu-id="2843a-p105">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2843a-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2843a-129">权限类型</span><span class="sxs-lookup"><span data-stu-id="2843a-129">Permission type</span></span>      | <span data-ttu-id="2843a-130">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2843a-130">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2843a-131">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2843a-131">Delegated (work or school account)</span></span> | <span data-ttu-id="2843a-132">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2843a-132">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2843a-133">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2843a-133">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2843a-134">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2843a-134">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="2843a-135">应用程序</span><span class="sxs-lookup"><span data-stu-id="2843a-135">Application</span></span> | <span data-ttu-id="2843a-136">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2843a-136">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2843a-137">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2843a-137">HTTP request</span></span>

<span data-ttu-id="2843a-138">本节显示初始 **delta** 函数调用的 HTTP 请求语法，以启动检索指定日历或日历视图中的所有事件的完全同步。</span><span class="sxs-lookup"><span data-stu-id="2843a-138">This section shows the HTTP request syntax for the initial **delta** function call to start a full synchronization that retrieves all the events in the specified calendar or calendar view.</span></span> <span data-ttu-id="2843a-139">此语法不包含任何 [状态令牌](/graph/delta-query-overview#state-tokens)。</span><span class="sxs-lookup"><span data-stu-id="2843a-139">This syntax does not contain any [state tokens](/graph/delta-query-overview#state-tokens).</span></span> 

<span data-ttu-id="2843a-140">在成功响应或成功响应中返回的查询 URL `nextLink` `deltaLink` 包括状态令牌。</span><span class="sxs-lookup"><span data-stu-id="2843a-140">The query URL returned in a `nextLink` or `deltaLink` of a successful response includes a state token.</span></span> <span data-ttu-id="2843a-141">对于任何后续 **delta** 函数调用，请使用查询 URL 中的或 `nextLink` `deltaLink` 前面的查询 URL。</span><span class="sxs-lookup"><span data-stu-id="2843a-141">For any subsequent **delta** function call, use the query URL in a `nextLink` or `deltaLink` preceding it.</span></span>

### <a name="delta-function-on-events-in-a-user-calendar-preview"></a><span data-ttu-id="2843a-142">用户日历中事件的 Delta 函数 (预览) </span><span class="sxs-lookup"><span data-stu-id="2843a-142">Delta function on events in a user calendar (preview)</span></span>
<span data-ttu-id="2843a-143">将 **delta** 函数应用于从特定日期/时间开始或之后的所有事件，在指定的用户日历 () ：</span><span class="sxs-lookup"><span data-stu-id="2843a-143">Apply the **delta** function on all the events or events starting on or after a specific date/time, in the specified user calendar(s):</span></span>

* <span data-ttu-id="2843a-144">若要获取用户邮箱中所有事件或自指定日期/时间之后开始的事件的增量 _更改，请执行以下操作_：</span><span class="sxs-lookup"><span data-stu-id="2843a-144">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's mailbox_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/events/delta 
  GET /users/{id | userPrincipalName}/events/delta 

  GET /me/events/delta?startDateTime={start_datetime}
  GET /users/{id | userPrincipalName}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="2843a-145">若要获取用户默认日历中指定日期/时间或之后开始的所有事件或事件的增量 _更改：_</span><span class="sxs-lookup"><span data-stu-id="2843a-145">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendar/events/delta 
  GET /users/{id | userPrincipalName}/calendar/events/delta 

  GET /me/calendar/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendar/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="2843a-146">若要获取指定用户日历中指定日期/时间或之后开始的所有事件或 _事件的增量更改_：</span><span class="sxs-lookup"><span data-stu-id="2843a-146">To get incremental changes of all the events, or of events starting on or after the specified date/time _in the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/events/delta 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta 

  GET /me/calendars/{id}/events/delta?startDateTime={start_datetime} 
  GET /users/{id | userPrincipalName}/calendars/{id}/events/delta?startDateTime={start_datetime}
  ```

* <span data-ttu-id="2843a-147">若要获取指定日历组和日历中指定日期/时间或之后开始的所有事件或事件的增量 _更改_：</span><span class="sxs-lookup"><span data-stu-id="2843a-147">To get incremental changes all the events, or of events starting on or after the specified date/time _in the specified calendar group and calendar_:</span></span>
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

### <a name="delta-function-on-calendarview-in-a-user-calendar"></a><span data-ttu-id="2843a-148">用户日历中 calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-148">Delta function on calendarView in a user calendar</span></span>
<span data-ttu-id="2843a-149">在 **指定的用户** 日历中，对以开始日期和结束日期/时间分隔的事件范围应用 delta 函数：</span><span class="sxs-lookup"><span data-stu-id="2843a-149">Apply the **delta** function on a range of events delimited by start and end date/times, in the specified user calendar:</span></span>

* <span data-ttu-id="2843a-150">若要在用户的默认日历的日历视图中获取增量 _更改，请执行以下操作_：</span><span class="sxs-lookup"><span data-stu-id="2843a-150">To get incremental changes in a calendar view of _the user's default calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

* <span data-ttu-id="2843a-151">若要获取指定用户日历的日历视图中 _的增量更改，请执行以下操作_：</span><span class="sxs-lookup"><span data-stu-id="2843a-151">To get incremental changes in a calendar view of _the specified user calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /me/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  GET /users/{id}/calendars/{id}/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

### <a name="delta-function-on-calendarview-in-a-group-calendar"></a><span data-ttu-id="2843a-152">组日历中 calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-152">Delta function on calendarView in a group calendar</span></span>
* <span data-ttu-id="2843a-153">若要在组日历的日历视图中 _获取增量更改，请执行_：</span><span class="sxs-lookup"><span data-stu-id="2843a-153">To get incremental changes in a calendar view of _a group's calendar_:</span></span>
  <!-- { "blockType": "ignored" } -->
  ```http
  GET /groups/{id}/calendarView?startDateTime={start_datetime}&endDateTime={end_datetime}
  ```

## <a name="query-parameters"></a><span data-ttu-id="2843a-154">查询参数</span><span class="sxs-lookup"><span data-stu-id="2843a-154">Query parameters</span></span>

<span data-ttu-id="2843a-155">跟踪更改将引发一轮或多次 **delta** 函数调用。</span><span class="sxs-lookup"><span data-stu-id="2843a-155">Tracking changes incurs a round of one or more **delta** function calls.</span></span> <span data-ttu-id="2843a-156">如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。</span><span class="sxs-lookup"><span data-stu-id="2843a-156">If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request.</span></span> <span data-ttu-id="2843a-157">Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。</span><span class="sxs-lookup"><span data-stu-id="2843a-157">Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response.</span></span> <span data-ttu-id="2843a-158">只需预先指定所需的任何查询参数一次。</span><span class="sxs-lookup"><span data-stu-id="2843a-158">You only need to specify any desired query parameters once upfront.</span></span>
<span data-ttu-id="2843a-159">在后续请求中，只需复制和应用上一响应中的或 `nextLink` `deltaLink` URL，因为该 URL 已包含编码的所需参数。</span><span class="sxs-lookup"><span data-stu-id="2843a-159">In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>

| <span data-ttu-id="2843a-160">查询参数</span><span class="sxs-lookup"><span data-stu-id="2843a-160">Query parameter</span></span>      | <span data-ttu-id="2843a-161">类型</span><span class="sxs-lookup"><span data-stu-id="2843a-161">Type</span></span>   |<span data-ttu-id="2843a-162">说明</span><span class="sxs-lookup"><span data-stu-id="2843a-162">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2843a-163">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2843a-163">startDateTime</span></span>|<span data-ttu-id="2843a-164">String</span><span class="sxs-lookup"><span data-stu-id="2843a-164">String</span></span>|<span data-ttu-id="2843a-p109">时间范围的开始日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T19:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="2843a-p109">The start date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T19:00:00-08:00". </span></span><br><span data-ttu-id="2843a-167">时区在参数值的时区偏移部分中指定，如果存在，则不会影响 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="2843a-167">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="2843a-168">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="2843a-168">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="2843a-169">对于 **日历中的事件** 增量，可选。</span><span class="sxs-lookup"><span data-stu-id="2843a-169">Optional for **delta** on events in a calendar.</span></span> <br><span data-ttu-id="2843a-170">在 **calendarView** 上 delta **是必需的**。</span><span class="sxs-lookup"><span data-stu-id="2843a-170">Required for **delta** on **calendarView**.</span></span> |
|<span data-ttu-id="2843a-171">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2843a-171">endDateTime</span></span>|<span data-ttu-id="2843a-172">String</span><span class="sxs-lookup"><span data-stu-id="2843a-172">String</span></span>|<span data-ttu-id="2843a-p111">时间范围的结束日期和时间，以 ISO 8601 格式表示。例如，“2019-11-08T20:00:00-08:00”。</span><span class="sxs-lookup"><span data-stu-id="2843a-p111">The end date and time of the time range, represented in ISO 8601 format. For example, "2019-11-08T20:00:00-08:00". </span></span><br><span data-ttu-id="2843a-175">时区在参数值的时区偏移部分中指定，如果存在，则不会影响 `Prefer: outlook.timezone` 标头。</span><span class="sxs-lookup"><span data-stu-id="2843a-175">The timezone is specified in the timezone offset portion of the parameter value, and is not impacted by the `Prefer: outlook.timezone` header if present.</span></span> <span data-ttu-id="2843a-176">如果值中未包含时区偏移量，则将其解释为 UTC。</span><span class="sxs-lookup"><span data-stu-id="2843a-176">If no timezone offset is included in the value, it is interpreted as UTC.</span></span><br><span data-ttu-id="2843a-177">_不受_**日历中事件** 上的 delta 支持。</span><span class="sxs-lookup"><span data-stu-id="2843a-177">_Not supported_ by **delta** on events in a calendar.</span></span> <br><span data-ttu-id="2843a-178">在 **calendarView** 上为 **delta 所必需**。</span><span class="sxs-lookup"><span data-stu-id="2843a-178">Required for **delta** on **calendarView**.</span></span>|
| <span data-ttu-id="2843a-179">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="2843a-179">$deltatoken</span></span> | <span data-ttu-id="2843a-180">string</span><span class="sxs-lookup"><span data-stu-id="2843a-180">string</span></span> | <span data-ttu-id="2843a-p113">对同一个日历视图之前的 **delta** 函数调用的 `deltaLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该日历视图的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="2843a-p113">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="2843a-183">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="2843a-183">$skiptoken</span></span> | <span data-ttu-id="2843a-184">string</span><span class="sxs-lookup"><span data-stu-id="2843a-184">string</span></span> | <span data-ttu-id="2843a-185">之前的 **delta** 函数调用的 `nextLink` URL 中返回的 [状态令牌](/graph/delta-query-overview)，指示同一个日历视图中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="2843a-185">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="2843a-186">不支持 `$expand` 、 `$filter` 、 和 `$orderby` `$select` `$search` 。</span><span class="sxs-lookup"><span data-stu-id="2843a-186">Does not support `$expand`, `$filter`, `$orderby`, `$select`, and `$search`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="2843a-187">请求标头</span><span class="sxs-lookup"><span data-stu-id="2843a-187">Request headers</span></span>
| <span data-ttu-id="2843a-188">名称</span><span class="sxs-lookup"><span data-stu-id="2843a-188">Name</span></span>       | <span data-ttu-id="2843a-189">类型</span><span class="sxs-lookup"><span data-stu-id="2843a-189">Type</span></span> | <span data-ttu-id="2843a-190">说明</span><span class="sxs-lookup"><span data-stu-id="2843a-190">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="2843a-191">Authorization</span><span class="sxs-lookup"><span data-stu-id="2843a-191">Authorization</span></span>  | <span data-ttu-id="2843a-192">string</span><span class="sxs-lookup"><span data-stu-id="2843a-192">string</span></span>  | <span data-ttu-id="2843a-p114">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2843a-p114">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2843a-195">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2843a-195">Content-Type</span></span>  | <span data-ttu-id="2843a-196">string</span><span class="sxs-lookup"><span data-stu-id="2843a-196">string</span></span>  | <span data-ttu-id="2843a-p115">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2843a-p115">application/json. Required.</span></span> |
| <span data-ttu-id="2843a-199">Prefer</span><span class="sxs-lookup"><span data-stu-id="2843a-199">Prefer</span></span> | <span data-ttu-id="2843a-200">string</span><span class="sxs-lookup"><span data-stu-id="2843a-200">string</span></span>  | <span data-ttu-id="2843a-p116">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="2843a-p116">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="2843a-203">Prefer</span><span class="sxs-lookup"><span data-stu-id="2843a-203">Prefer</span></span> | <span data-ttu-id="2843a-204">string</span><span class="sxs-lookup"><span data-stu-id="2843a-204">string</span></span> | <span data-ttu-id="2843a-205">outlook.timezone={时区字符串}。</span><span class="sxs-lookup"><span data-stu-id="2843a-205">outlook.timezone={Time zone string}.</span></span> <span data-ttu-id="2843a-206">可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="2843a-206">Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="2843a-207">响应</span><span class="sxs-lookup"><span data-stu-id="2843a-207">Response</span></span>

### <a name="delta-function-on-events-preview"></a><span data-ttu-id="2843a-208">事件上的 Delta 函数 (预览) </span><span class="sxs-lookup"><span data-stu-id="2843a-208">Delta function on events (preview)</span></span>
<span data-ttu-id="2843a-209">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和事件集合。 [](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="2843a-209">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span> <span data-ttu-id="2843a-210">出于 **性能** 原因，响应中的每个事件仅包含 **ID、\*\*\*\*类型\*\*\*\*、** 开始和结束属性。</span><span class="sxs-lookup"><span data-stu-id="2843a-210">Each **event** in the response contains only the **id**, **type**, **start** and **end** properties for performance reasons.</span></span> <span data-ttu-id="2843a-211">随后 `GET /events/{id}` 使用扩展响应中的任意事件。</span><span class="sxs-lookup"><span data-stu-id="2843a-211">Use `GET /events/{id}` subsequently to expand any events from the response.</span></span>  

### <a name="delta-function-on-calendarview"></a><span data-ttu-id="2843a-212">calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-212">Delta function on calendarView</span></span>
<span data-ttu-id="2843a-213">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和事件集合。 [](../resources/event.md)</span><span class="sxs-lookup"><span data-stu-id="2843a-213">If successful, this method returns a `200 OK` response code and an [event](../resources/event.md) collection in the response body.</span></span>

<span data-ttu-id="2843a-214">期望获取通常从请求获取的所有 `GET /calendarview` 属性。</span><span class="sxs-lookup"><span data-stu-id="2843a-214">Expect to get all the properties you'd normally get from a `GET /calendarview` request.</span></span> 

## <a name="examples"></a><span data-ttu-id="2843a-215">示例</span><span class="sxs-lookup"><span data-stu-id="2843a-215">Examples</span></span>

### <a name="example-1-delta-function-on-events-in-a-calendar-preview"></a><span data-ttu-id="2843a-216">示例 1：日历中事件的 Delta 函数 (预览) </span><span class="sxs-lookup"><span data-stu-id="2843a-216">Example 1: Delta function on events in a calendar (preview)</span></span>
#### <a name="request"></a><span data-ttu-id="2843a-217">请求</span><span class="sxs-lookup"><span data-stu-id="2843a-217">Request</span></span>
<span data-ttu-id="2843a-218">以下示例显示用于获取已登录用户的默认日历中的事件的初始同步请求，该事件发生在指定参数上或之后 `startDateTime` 。</span><span class="sxs-lookup"><span data-stu-id="2843a-218">The following example shows the initial sync request to get events in the signed-in user's default calendar, that occur on or after the specified `startDateTime` parameter.</span></span> <span data-ttu-id="2843a-219">初始请求不包括任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="2843a-219">The initial request does not include any state token.</span></span> 

<span data-ttu-id="2843a-220">请求使用标头将每个响应中的最大事件数限制为 `Prefer: odata.maxpagesize` 1。</span><span class="sxs-lookup"><span data-stu-id="2843a-220">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 1.</span></span> <span data-ttu-id="2843a-221">继续使用 `delta` 返回的查询调用函数， `@odata.nextLink` 直到收到 `@odata.deltaLink` 响应。</span><span class="sxs-lookup"><span data-stu-id="2843a-221">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get a `@odata.deltaLink` in the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta_events"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendar/events/delta?startDateTime=2020-06-12T00:00:00Z

Prefer: odata.maxpagesize=1
```

#### <a name="response"></a><span data-ttu-id="2843a-222">响应</span><span class="sxs-lookup"><span data-stu-id="2843a-222">Response</span></span>

<span data-ttu-id="2843a-223">如果请求成功，响应将包含状态令牌，该令牌是 _\@ odata.nextLink_ 响应标头) 中的 _skipToken_ (或 _\@ odata.deltaLink_ 响应标头) 中的 _deltaToken_ (。</span><span class="sxs-lookup"><span data-stu-id="2843a-223">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="2843a-224">它们分别指示是继续该轮，还是已完成获取该轮的所有更改。</span><span class="sxs-lookup"><span data-stu-id="2843a-224">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="2843a-225">下面的响应在 _\@ odata.nextLink_ 响应标头中显示 _skipToken。_</span><span class="sxs-lookup"><span data-stu-id="2843a-225">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

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


### <a name="example-2-delta-function-on-calendarview"></a><span data-ttu-id="2843a-226">示例 2：calendarView 上的 Delta 函数</span><span class="sxs-lookup"><span data-stu-id="2843a-226">Example 2: Delta function on calendarView</span></span>
#### <a name="request"></a><span data-ttu-id="2843a-227">请求</span><span class="sxs-lookup"><span data-stu-id="2843a-227">Request</span></span>

<span data-ttu-id="2843a-228">以下示例显示获取已登录用户指定日历中的事件的初始同步请求，该同步请求在 **calendarView** 指示的日期范围内。</span><span class="sxs-lookup"><span data-stu-id="2843a-228">The following example shows the initial sync request to get events in the specified calendar of the signed-in user, within the range of dates indicated by the **calendarView**.</span></span> <span data-ttu-id="2843a-229">初始请求不包括任何状态令牌。</span><span class="sxs-lookup"><span data-stu-id="2843a-229">The initial request does not include any state token.</span></span> 

<span data-ttu-id="2843a-230">请求使用 `Prefer: odata.maxpagesize` 标头将每个响应中的最大事件数限制为 2。</span><span class="sxs-lookup"><span data-stu-id="2843a-230">The request uses the `Prefer: odata.maxpagesize` header to limit the maximum number of events in each response to 2.</span></span> <span data-ttu-id="2843a-231">继续使用返回的查询调用函数，直到获取该日历视图中的所有事件和 `delta` `@odata.nextLink` 响应 `@odata.deltaLink` 中的 a。</span><span class="sxs-lookup"><span data-stu-id="2843a-231">Continue calling the `delta` function by using the query returned in `@odata.nextLink` until you get all the events in that calendar view, and a `@odata.deltaLink` in the response.</span></span>

# <a name="http"></a>[<span data-ttu-id="2843a-232">HTTP</span><span class="sxs-lookup"><span data-stu-id="2843a-232">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["AAMkADI5M1BbeAAA="],
  "name": "event_delta_calendarview"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/calendars/AAMkADI5M1BbeAAA=/calendarview/delta?startDateTime=2020-06-01T00:00:00Z&endDateTime=2020-06-10T00:00:00Z

Prefer: odata.maxpagesize=2
```
# <a name="c"></a>[<span data-ttu-id="2843a-233">C#</span><span class="sxs-lookup"><span data-stu-id="2843a-233">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/event-delta-calendarview-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2843a-234">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2843a-234">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/event-delta-calendarview-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2843a-235">Java</span><span class="sxs-lookup"><span data-stu-id="2843a-235">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/event-delta-calendarview-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2843a-236">响应</span><span class="sxs-lookup"><span data-stu-id="2843a-236">Response</span></span>

<span data-ttu-id="2843a-237">如果请求成功，响应将包含状态令牌，该令牌是 _\@ odata.nextLink_ 响应标头) 中的 _skipToken_ (或 _\@ odata.deltaLink_ 响应标头 (中的 _deltaToken_) 。</span><span class="sxs-lookup"><span data-stu-id="2843a-237">If the request is successful, the response includes a state token, which is either a _skipToken_ (in an _\@odata.nextLink_ response header) or a _deltaToken_ (in an _\@odata.deltaLink_ response header).</span></span>
<span data-ttu-id="2843a-238">它们分别指示是继续该轮，还是已完成获取该轮的所有更改。</span><span class="sxs-lookup"><span data-stu-id="2843a-238">Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="2843a-239">下面的响应在 _\@ odata.nextLink_ 响应标头中显示 _skipToken。_</span><span class="sxs-lookup"><span data-stu-id="2843a-239">The response below shows a _skipToken_ in an _\@odata.nextLink_ response header.</span></span>

<span data-ttu-id="2843a-240">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2843a-240">Note: The response object shown here may be truncated for brevity.</span></span> 
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

## <a name="see-also"></a><span data-ttu-id="2843a-241">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2843a-241">See also</span></span>

- [<span data-ttu-id="2843a-242">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="2843a-242">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="2843a-243">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="2843a-243">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

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


