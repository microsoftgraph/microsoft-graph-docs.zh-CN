---
title: 'event: delta'
description: 获取在**calendarView**中添加、删除或更新的一组事件 (事件范围)
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: e04e542e0bf119e28a000f1b7fed3777590c1654
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464441"
---
# <a name="event-delta"></a><span data-ttu-id="68a24-103">event: delta</span><span class="sxs-lookup"><span data-stu-id="68a24-103">event: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68a24-104">获取用户主日历的 **calendarView**（事件范围）中已添加、删除或更新的事件集。</span><span class="sxs-lookup"><span data-stu-id="68a24-104">Get a set of events that have been added, deleted, or updated in a **calendarView** (a range of events) of the user's primary calendar.</span></span>

<span data-ttu-id="68a24-p101">对于用户主日历的日期范围，对事件的 **delta** 函数调用与 `GET /calendarview` 请求相似，但是可通过在对其的一次或多次调用中正确应用[状态令牌](/graph/delta-query-overview)来查询该日历视图中的增量更改这一点除外。通过此功能，你可以维护和同步本地存储的主日历的用户事件，而无需每次都从服务器中获取该日历的所有事件。</span><span class="sxs-lookup"><span data-stu-id="68a24-p101">A **delta** function call for events is similar to a `GET /calendarview` request for a range of dates in the user's primary calendar, except that by appropriately applying [state tokens](/graph/delta-query-overview) in one or more of these calls, you can query for incremental changes in that calender view. This allows you to maintain and synchronize a local store of a user's events in the primary calendar, without having to fetch all the events of that calendar from the server every time.</span></span>

## <a name="permissions"></a><span data-ttu-id="68a24-107">权限</span><span class="sxs-lookup"><span data-stu-id="68a24-107">Permissions</span></span>
<span data-ttu-id="68a24-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68a24-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="68a24-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="68a24-110">Permission type</span></span>      | <span data-ttu-id="68a24-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68a24-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68a24-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68a24-112">Delegated (work or school account)</span></span> | <span data-ttu-id="68a24-113">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68a24-113">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="68a24-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68a24-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68a24-115">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68a24-115">Calendars.Read, Calendars.ReadWrite</span></span>    |
|<span data-ttu-id="68a24-116">Application</span><span class="sxs-lookup"><span data-stu-id="68a24-116">Application</span></span> | <span data-ttu-id="68a24-117">Calendars.Read、Calendars.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="68a24-117">Calendars.Read, Calendars.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="68a24-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68a24-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}
GET /users/<id>/calendarView/delta?startDateTime={start_datetime}&endDateTime={end_datetime}

```

## <a name="query-parameters"></a><span data-ttu-id="68a24-119">查询参数</span><span class="sxs-lookup"><span data-stu-id="68a24-119">Query parameters</span></span>

<span data-ttu-id="68a24-p103">跟踪事件更改会引发一组对 **delta** 函数的一次或多次调用。如果要使用任意查询参数（`$deltatoken` 和 `$skiptoken` 除外），则必须在最初的 **delta** 请求中指定它。Microsoft Graph 自动将指定的任意参数编码为响应中提供的 `nextLink` 或 `deltaLink` URL 的令牌部分。你只需预先指定任意所需查询参数一次。在后续的请求中，只需复制并应用以前响应中的 `nextLink` 或 `deltaLink` URL，因为该 URL 已包含所需的编码参数。</span><span class="sxs-lookup"><span data-stu-id="68a24-p103">Tracking changes in events incurs a round of one or more **delta** function calls. If you use any query parameter (other than `$deltatoken` and `$skiptoken`), you must specify it in the initial **delta** request. Microsoft Graph automatically encodes any specified parameters into the token portion of the `nextLink` or `deltaLink` URL provided in the response. You only need to specify any desired query parameters once upfront. In subsequent requests, simply copy and apply the `nextLink` or `deltaLink` URL from the previous response, as that URL already includes the encoded, desired parameters.</span></span>


| <span data-ttu-id="68a24-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="68a24-125">Query parameter</span></span>      | <span data-ttu-id="68a24-126">类型</span><span class="sxs-lookup"><span data-stu-id="68a24-126">Type</span></span>   |<span data-ttu-id="68a24-127">说明</span><span class="sxs-lookup"><span data-stu-id="68a24-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="68a24-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="68a24-128">startDateTime</span></span>|<span data-ttu-id="68a24-129">字符串</span><span class="sxs-lookup"><span data-stu-id="68a24-129">String</span></span>|<span data-ttu-id="68a24-p104">时间范围的开始日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T19:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="68a24-p104">The start date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T19:00:00.0000000".</span></span>|
|<span data-ttu-id="68a24-132">endDateTime</span><span class="sxs-lookup"><span data-stu-id="68a24-132">endDateTime</span></span>|<span data-ttu-id="68a24-133">String</span><span class="sxs-lookup"><span data-stu-id="68a24-133">String</span></span>|<span data-ttu-id="68a24-p105">时间范围的结束日期和时间以 ISO 8601 格式表示。例如，“2015-11-08T20:00:00.0000000”。</span><span class="sxs-lookup"><span data-stu-id="68a24-p105">The end date and time of the time range, represented in ISO 8601 format. For example, "2015-11-08T20:00:00.0000000".</span></span>|
| <span data-ttu-id="68a24-136">$deltatoken</span><span class="sxs-lookup"><span data-stu-id="68a24-136">$deltatoken</span></span> | <span data-ttu-id="68a24-137">string</span><span class="sxs-lookup"><span data-stu-id="68a24-137">string</span></span> | <span data-ttu-id="68a24-p106">对同一个日历视图之前的 **delta** 函数调用的 `deltaLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示该组更改跟踪的完成状态。将此令牌包含在对该日历视图的下一组更改追踪的首次请求中，并保存和应用整个 `deltaLink` URL。</span><span class="sxs-lookup"><span data-stu-id="68a24-p106">A [state token](/graph/delta-query-overview) returned in the `deltaLink` URL of the previous **delta** function call for the same calendar view, indicating the completion of that round of change tracking. Save and apply the entire `deltaLink` URL including this token in the first request of the next round of change tracking for that calendar view.</span></span>|
| <span data-ttu-id="68a24-140">$skiptoken</span><span class="sxs-lookup"><span data-stu-id="68a24-140">$skiptoken</span></span> | <span data-ttu-id="68a24-141">字符串</span><span class="sxs-lookup"><span data-stu-id="68a24-141">string</span></span> | <span data-ttu-id="68a24-142">之前的 **delta** 函数调用的 `nextLink` URL 中返回的[状态令牌](/graph/delta-query-overview)，指示同一个日历视图中有进一步的更改需要跟踪。</span><span class="sxs-lookup"><span data-stu-id="68a24-142">A [state token](/graph/delta-query-overview) returned in the `nextLink` URL of the previous **delta** function call, indicating there are further changes to be tracked in the same calendar view.</span></span> |

<span data-ttu-id="68a24-p107">对日历视图执行 delta 查询时，预计获取通常从 `GET /calendarview` 请求获取的所有属性。在此情况下，不支持 `$select`。</span><span class="sxs-lookup"><span data-stu-id="68a24-p107">When you do a delta query on a calendar view, expect to get all the properties you'd normally get from a `GET /calendarview` request. `$select` is not supported in this case.</span></span>


## <a name="request-headers"></a><span data-ttu-id="68a24-145">请求头</span><span class="sxs-lookup"><span data-stu-id="68a24-145">Request headers</span></span>
| <span data-ttu-id="68a24-146">名称</span><span class="sxs-lookup"><span data-stu-id="68a24-146">Name</span></span>       | <span data-ttu-id="68a24-147">类型</span><span class="sxs-lookup"><span data-stu-id="68a24-147">Type</span></span> | <span data-ttu-id="68a24-148">说明</span><span class="sxs-lookup"><span data-stu-id="68a24-148">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="68a24-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="68a24-149">Authorization</span></span>  | <span data-ttu-id="68a24-150">string</span><span class="sxs-lookup"><span data-stu-id="68a24-150">string</span></span>  | <span data-ttu-id="68a24-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68a24-p108">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="68a24-153">Content-Type</span><span class="sxs-lookup"><span data-stu-id="68a24-153">Content-Type</span></span>  | <span data-ttu-id="68a24-154">string</span><span class="sxs-lookup"><span data-stu-id="68a24-154">string</span></span>  | <span data-ttu-id="68a24-p109">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="68a24-p109">application/json. Required.</span></span> |
| <span data-ttu-id="68a24-157">Prefer</span><span class="sxs-lookup"><span data-stu-id="68a24-157">Prefer</span></span> | <span data-ttu-id="68a24-158">字符串</span><span class="sxs-lookup"><span data-stu-id="68a24-158">string</span></span>  | <span data-ttu-id="68a24-p110">odata.maxpagesize={x}。可选。</span><span class="sxs-lookup"><span data-stu-id="68a24-p110">odata.maxpagesize={x}. Optional.</span></span> |
| <span data-ttu-id="68a24-161">Prefer</span><span class="sxs-lookup"><span data-stu-id="68a24-161">Prefer</span></span> | <span data-ttu-id="68a24-162">string</span><span class="sxs-lookup"><span data-stu-id="68a24-162">string</span></span> | <span data-ttu-id="68a24-p111">{Time zone}。可选，如果缺省，则采用 UTC。</span><span class="sxs-lookup"><span data-stu-id="68a24-p111">{Time zone}. Optional, UTC assumed if absent.</span></span>|

## <a name="response"></a><span data-ttu-id="68a24-165">响应</span><span class="sxs-lookup"><span data-stu-id="68a24-165">Response</span></span>

<span data-ttu-id="68a24-166">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [event](../resources/event.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="68a24-166">If successful, this method returns a `200 OK` response code and [event](../resources/event.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68a24-167">示例</span><span class="sxs-lookup"><span data-stu-id="68a24-167">Example</span></span>
##### <a name="request"></a><span data-ttu-id="68a24-168">请求</span><span class="sxs-lookup"><span data-stu-id="68a24-168">Request</span></span>

<span data-ttu-id="68a24-169">以下示例演示了如何执行单次 **delta** 函数调用，并将响应正文中的事件最大数目限制为 2。</span><span class="sxs-lookup"><span data-stu-id="68a24-169">The following example shows how to make a single **delta** function call, and limit the maximum number of events in the response body to 2.</span></span>

<span data-ttu-id="68a24-170">若要跟踪日历视图的更改，要使用正确的[状态令牌](/graph/delta-query-overview)执行一次或多次 **delta** 函数调用来获取上次增量查询后的增量更改集。</span><span class="sxs-lookup"><span data-stu-id="68a24-170">To track changes in a calendar view, you would make one or more **delta** function calls, with appropriate [state tokens](/graph/delta-query-overview), to get the set of incremental changes since the last delta query.</span></span>

<!-- {
  "blockType": "request",
  "name": "event_delta"
}-->
```http
GET https://graph.microsoft.com/beta/me/calendarview/delta?startdatetime={start_datetime}&enddatetime={end_datetime}

Prefer: odata.maxpagesize=2
```

##### <a name="response"></a><span data-ttu-id="68a24-171">响应</span><span class="sxs-lookup"><span data-stu-id="68a24-171">Response</span></span>
<span data-ttu-id="68a24-p112">如果请求成功，响应将包括状态令牌，即 _skipToken_（位于 _@odata.nextLink_ 响应头中）或 _deltaToken_（位于 _@odata.deltaLink_ 响应头中）。它们分别指示应继续此组调用还是已获取该组的所有更改。</span><span class="sxs-lookup"><span data-stu-id="68a24-p112">If the request is successful, the response would include a state token, which is either a _skipToken_ (in an _@odata.nextLink_ response header) or a _deltaToken_ (in an _@odata.deltaLink_ response header). Respectively, they indicate whether you should continue with the round or you have completed getting all the changes for that round.</span></span>

<span data-ttu-id="68a24-174">以下响应显示了 _@odata.nextLink_ 响应头中的 _skipToken_。</span><span class="sxs-lookup"><span data-stu-id="68a24-174">The response below shows a _skipToken_ in an _@odata.nextLink_ response header.</span></span>

<span data-ttu-id="68a24-p113">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="68a24-p113">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.event",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 359

{
  "@odata.nextLink":"https://graph.microsoft.com/beta/me/calendarview/delta?$skiptoken={_skipToken_}",
  "value": [
    {
      "originalStartTimeZone": "originalStartTimeZone-value",
      "originalEndTimeZone": "originalEndTimeZone-value",
      "responseStatus": {
        "response": "response-value",
        "time": "datetime-value"
      },
      "uid": "iCalUId-value",
      "reminderMinutesBeforeStart": 99,
      "isReminderOn": true
    }
  ]
}
```

### <a name="see-also"></a><span data-ttu-id="68a24-177">另请参阅</span><span class="sxs-lookup"><span data-stu-id="68a24-177">See also</span></span>

- [<span data-ttu-id="68a24-178">Microsoft Graph 增量查询</span><span class="sxs-lookup"><span data-stu-id="68a24-178">Microsoft Graph delta query</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="68a24-179">获取文件夹中事件的增量更改</span><span class="sxs-lookup"><span data-stu-id="68a24-179">Get incremental changes to events in a folder</span></span>](/graph/delta-query-events)

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
    "Error: /api-reference/beta/api/event-delta.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
