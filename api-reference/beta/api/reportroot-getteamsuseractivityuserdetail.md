---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: eba2f5d05a5571bf7f4fa4cd72d9a945b9936481
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766397"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="da400-103">reportRoot: getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="da400-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

<span data-ttu-id="da400-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da400-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da400-105">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="da400-105">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="da400-106">权限</span><span class="sxs-lookup"><span data-stu-id="da400-106">Permissions</span></span>

<span data-ttu-id="da400-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da400-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="da400-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="da400-109">Permission type</span></span>                        | <span data-ttu-id="da400-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da400-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="da400-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da400-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="da400-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da400-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="da400-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da400-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da400-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="da400-114">Not supported.</span></span>                           |
| <span data-ttu-id="da400-115">应用</span><span class="sxs-lookup"><span data-stu-id="da400-115">Application</span></span>                            | <span data-ttu-id="da400-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="da400-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="da400-117">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="da400-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="da400-118">有关更多详细信息，请参阅[授权 API 读取 Microsoft 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="da400-118">For more details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="da400-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da400-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="da400-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="da400-120">Function parameters</span></span>

<span data-ttu-id="da400-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="da400-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="da400-122">参数</span><span class="sxs-lookup"><span data-stu-id="da400-122">Parameter</span></span> | <span data-ttu-id="da400-123">类型</span><span class="sxs-lookup"><span data-stu-id="da400-123">Type</span></span>   | <span data-ttu-id="da400-124">说明</span><span class="sxs-lookup"><span data-stu-id="da400-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="da400-125">period</span><span class="sxs-lookup"><span data-stu-id="da400-125">period</span></span>    | <span data-ttu-id="da400-126">string</span><span class="sxs-lookup"><span data-stu-id="da400-126">string</span></span> | <span data-ttu-id="da400-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="da400-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="da400-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="da400-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="da400-129">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="da400-129">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="da400-130">date</span><span class="sxs-lookup"><span data-stu-id="da400-130">date</span></span>      | <span data-ttu-id="da400-131">Date</span><span class="sxs-lookup"><span data-stu-id="da400-131">Date</span></span>   | <span data-ttu-id="da400-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="da400-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="da400-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="da400-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="da400-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="da400-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="da400-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="da400-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="da400-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da400-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="da400-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="da400-137">The default output type is text/csv.</span></span> <span data-ttu-id="da400-138">但是，如果要指定输出类型，可以使用 OData 查询参数$format text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="da400-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da400-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="da400-139">Request headers</span></span>

| <span data-ttu-id="da400-140">名称</span><span class="sxs-lookup"><span data-stu-id="da400-140">Name</span></span>          | <span data-ttu-id="da400-141">说明</span><span class="sxs-lookup"><span data-stu-id="da400-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="da400-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="da400-142">Authorization</span></span> | <span data-ttu-id="da400-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da400-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="da400-145">响应</span><span class="sxs-lookup"><span data-stu-id="da400-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="da400-146">CSV</span><span class="sxs-lookup"><span data-stu-id="da400-146">CSV</span></span>

<span data-ttu-id="da400-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="da400-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="da400-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="da400-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="da400-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="da400-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="da400-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="da400-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="da400-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="da400-151">Report Refresh Date</span></span>
- <span data-ttu-id="da400-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="da400-152">User Principal Name</span></span>
- <span data-ttu-id="da400-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="da400-153">Last Activity Date</span></span>
- <span data-ttu-id="da400-154">已删除</span><span class="sxs-lookup"><span data-stu-id="da400-154">Is Deleted</span></span>
- <span data-ttu-id="da400-155">删除日期</span><span class="sxs-lookup"><span data-stu-id="da400-155">Deleted Date</span></span>
- <span data-ttu-id="da400-156">分配的产品</span><span class="sxs-lookup"><span data-stu-id="da400-156">Assigned Products</span></span>
- <span data-ttu-id="da400-157">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="da400-157">Team Chat Message Count</span></span>
- <span data-ttu-id="da400-158">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="da400-158">Private Chat Message Count</span></span>
- <span data-ttu-id="da400-159">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="da400-159">Call Count</span></span>
- <span data-ttu-id="da400-160">会议计数</span><span class="sxs-lookup"><span data-stu-id="da400-160">Meeting Count</span></span>
- <span data-ttu-id="da400-161">会议组织计数</span><span class="sxs-lookup"><span data-stu-id="da400-161">Meetings Organized Count</span></span>
- <span data-ttu-id="da400-162">会议参加计数</span><span class="sxs-lookup"><span data-stu-id="da400-162">Meetings Attended Count</span></span>
- <span data-ttu-id="da400-163">临时会议组织计数</span><span class="sxs-lookup"><span data-stu-id="da400-163">Ad Hoc Meetings Organized Count</span></span>
- <span data-ttu-id="da400-164">参加临时会议计数</span><span class="sxs-lookup"><span data-stu-id="da400-164">Ad Hoc Meetings Attended Count</span></span>
- <span data-ttu-id="da400-165">安排的一次会议组织计数</span><span class="sxs-lookup"><span data-stu-id="da400-165">Scheduled One-time Meetings Organized Count</span></span>
- <span data-ttu-id="da400-166">已安排的一次会议参加次数</span><span class="sxs-lookup"><span data-stu-id="da400-166">Scheduled One-time Meetings Attended Count</span></span>
- <span data-ttu-id="da400-167">安排的定期会议组织计数</span><span class="sxs-lookup"><span data-stu-id="da400-167">Scheduled Recurring Meetings Organized Count</span></span>
- <span data-ttu-id="da400-168">已安排的定期会议参加次数</span><span class="sxs-lookup"><span data-stu-id="da400-168">Scheduled Recurring Meetings Attended Count</span></span>
- <span data-ttu-id="da400-169">音频持续时间</span><span class="sxs-lookup"><span data-stu-id="da400-169">Audio Duration</span></span>
- <span data-ttu-id="da400-170">视频持续时间</span><span class="sxs-lookup"><span data-stu-id="da400-170">Video Duration</span></span>
- <span data-ttu-id="da400-171">屏幕共享持续时间</span><span class="sxs-lookup"><span data-stu-id="da400-171">Screen Share Duration</span></span>
- <span data-ttu-id="da400-172">音频持续时间（以秒数表示）</span><span class="sxs-lookup"><span data-stu-id="da400-172">Audio Duration In Seconds</span></span>
- <span data-ttu-id="da400-173">视频持续时间（秒）</span><span class="sxs-lookup"><span data-stu-id="da400-173">Video Duration In Seconds</span></span>
- <span data-ttu-id="da400-174">屏幕共享持续时间（秒）</span><span class="sxs-lookup"><span data-stu-id="da400-174">Screen Share Duration In Seconds</span></span>
- <span data-ttu-id="da400-175">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="da400-175">Has Other Action</span></span>
- <span data-ttu-id="da400-176">已许可</span><span class="sxs-lookup"><span data-stu-id="da400-176">Is Licensed</span></span>
- <span data-ttu-id="da400-177">报表周期</span><span class="sxs-lookup"><span data-stu-id="da400-177">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="da400-178">JSON</span><span class="sxs-lookup"><span data-stu-id="da400-178">JSON</span></span>

<span data-ttu-id="da400-179">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="da400-179">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="da400-180">此请求的默认页面大小为 2000 个项目。</span><span class="sxs-lookup"><span data-stu-id="da400-180">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="da400-181">示例</span><span class="sxs-lookup"><span data-stu-id="da400-181">Example</span></span>

### <a name="csv"></a><span data-ttu-id="da400-182">CSV</span><span class="sxs-lookup"><span data-stu-id="da400-182">CSV</span></span>

<span data-ttu-id="da400-183">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="da400-183">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="da400-184">请求</span><span class="sxs-lookup"><span data-stu-id="da400-184">Request</span></span>

<span data-ttu-id="da400-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da400-185">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```


#### <a name="response"></a><span data-ttu-id="da400-186">响应</span><span class="sxs-lookup"><span data-stu-id="da400-186">Response</span></span>

<span data-ttu-id="da400-187">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da400-187">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="da400-188">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="da400-188">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Meetings Organized Count,Meetings Attended Count,Ad Hoc Meetings Organized Count,Ad Hoc Meetings Attended Count,Scheduled One-time Meetings Organized Count,Scheduled One-time Meetings Attended Count,Scheduled Recurring Meetings Organized Count,Scheduled Recurring Meetings Attended Count,Audio Duration,Video Duration,Screen Share Duration,Audio Duration In Seconds,Video Duration In Seconds,Screen Share Duration In Seconds,Has Other Action,Is Licensed,Report Period
```

### <a name="json"></a><span data-ttu-id="da400-189">JSON</span><span class="sxs-lookup"><span data-stu-id="da400-189">JSON</span></span>

<span data-ttu-id="da400-190">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="da400-190">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="da400-191">请求</span><span class="sxs-lookup"><span data-stu-id="da400-191">Request</span></span>

<span data-ttu-id="da400-192">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da400-192">The following is an example of the request.</span></span>


<!-- {
  "blockType": "ignored",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```


#### <a name="response"></a><span data-ttu-id="da400-193">响应</span><span class="sxs-lookup"><span data-stu-id="da400-193">Response</span></span>

<span data-ttu-id="da400-194">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da400-194">The following is an example of the response.</span></span>

> <span data-ttu-id="da400-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="da400-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsUserActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 452

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsUserActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "isLicensed": true, 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "Microsoft 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "meetingsOrganizedCount": 0, 
      "meetingsAttendedCount": 0, 
      "adHocMeetingsOrganizedCount": 0, 
      "adHocMeetingsAttendedCount": 0, 
      "scheduledOneTimeMeetingsOrganizedCount": 0, 
      "scheduledOneTimeMeetingsAttendedCount": 0, 
      "scheduledRecurringMeetingsOrganizedCount": 0, 
      "scheduledRecurringMeetingsAttendedCount": 0, 
      "audioDuration": 00:00:00, 
      "videoDuration": 00:00:00, 
      "screenShareDuration": 00:00:00, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


