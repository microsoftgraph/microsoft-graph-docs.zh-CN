---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 453be7fcb51aecf3bfd237b0d65708341f169b8b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639094"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="1ba8f-103">reportRoot：getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="1ba8f-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ba8f-104">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ba8f-105">权限</span><span class="sxs-lookup"><span data-stu-id="1ba8f-105">Permissions</span></span>

<span data-ttu-id="1ba8f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1ba8f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1ba8f-108">Permission type</span></span>                        | <span data-ttu-id="1ba8f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1ba8f-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1ba8f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba8f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="1ba8f-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ba8f-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1ba8f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1ba8f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ba8f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-113">Not supported.</span></span>                           |
| <span data-ttu-id="1ba8f-114">应用</span><span class="sxs-lookup"><span data-stu-id="1ba8f-114">Application</span></span>                            | <span data-ttu-id="1ba8f-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ba8f-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1ba8f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1ba8f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="1ba8f-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-117">Function parameters</span></span>

<span data-ttu-id="1ba8f-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="1ba8f-119">参数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-119">Parameter</span></span> | <span data-ttu-id="1ba8f-120">类型</span><span class="sxs-lookup"><span data-stu-id="1ba8f-120">Type</span></span>   | <span data-ttu-id="1ba8f-121">说明</span><span class="sxs-lookup"><span data-stu-id="1ba8f-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1ba8f-122">period</span><span class="sxs-lookup"><span data-stu-id="1ba8f-122">period</span></span>    | <span data-ttu-id="1ba8f-123">string</span><span class="sxs-lookup"><span data-stu-id="1ba8f-123">string</span></span> | <span data-ttu-id="1ba8f-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1ba8f-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1ba8f-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="1ba8f-127">date</span><span class="sxs-lookup"><span data-stu-id="1ba8f-127">date</span></span>      | <span data-ttu-id="1ba8f-128">Date</span><span class="sxs-lookup"><span data-stu-id="1ba8f-128">Date</span></span>   | <span data-ttu-id="1ba8f-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="1ba8f-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="1ba8f-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="1ba8f-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="1ba8f-133">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1ba8f-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-134">The default output type is text/csv.</span></span> <span data-ttu-id="1ba8f-135">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ba8f-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="1ba8f-136">Request headers</span></span>

| <span data-ttu-id="1ba8f-137">名称</span><span class="sxs-lookup"><span data-stu-id="1ba8f-137">Name</span></span>          | <span data-ttu-id="1ba8f-138">说明</span><span class="sxs-lookup"><span data-stu-id="1ba8f-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1ba8f-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba8f-139">Authorization</span></span> | <span data-ttu-id="1ba8f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1ba8f-142">响应</span><span class="sxs-lookup"><span data-stu-id="1ba8f-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1ba8f-143">CSV</span><span class="sxs-lookup"><span data-stu-id="1ba8f-143">CSV</span></span>

<span data-ttu-id="1ba8f-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1ba8f-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1ba8f-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1ba8f-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1ba8f-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1ba8f-148">Report Refresh Date</span></span>
- <span data-ttu-id="1ba8f-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1ba8f-149">User Principal Name</span></span>
- <span data-ttu-id="1ba8f-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="1ba8f-150">Last Activity Date</span></span>
- <span data-ttu-id="1ba8f-151">已删除</span><span class="sxs-lookup"><span data-stu-id="1ba8f-151">Is Deleted</span></span>
- <span data-ttu-id="1ba8f-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="1ba8f-152">Deleted Date</span></span>
- <span data-ttu-id="1ba8f-153">分配的产品</span><span class="sxs-lookup"><span data-stu-id="1ba8f-153">Assigned Products</span></span>
- <span data-ttu-id="1ba8f-154">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-154">Team Chat Message Count</span></span>
- <span data-ttu-id="1ba8f-155">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-155">Private Chat Message Count</span></span>
- <span data-ttu-id="1ba8f-156">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-156">Call Count</span></span>
- <span data-ttu-id="1ba8f-157">会议计数</span><span class="sxs-lookup"><span data-stu-id="1ba8f-157">Meeting Count</span></span>
- <span data-ttu-id="1ba8f-158">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="1ba8f-158">Has Other Action</span></span>
- <span data-ttu-id="1ba8f-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="1ba8f-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1ba8f-160">JSON</span><span class="sxs-lookup"><span data-stu-id="1ba8f-160">JSON</span></span>

<span data-ttu-id="1ba8f-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-161">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="1ba8f-162">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="1ba8f-163">示例</span><span class="sxs-lookup"><span data-stu-id="1ba8f-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1ba8f-164">CSV</span><span class="sxs-lookup"><span data-stu-id="1ba8f-164">CSV</span></span>

<span data-ttu-id="1ba8f-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1ba8f-166">请求</span><span class="sxs-lookup"><span data-stu-id="1ba8f-166">Request</span></span>

<span data-ttu-id="1ba8f-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1ba8f-168">响应</span><span class="sxs-lookup"><span data-stu-id="1ba8f-168">Response</span></span>

<span data-ttu-id="1ba8f-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ba8f-170">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1ba8f-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ba8f-171">语言</span><span class="sxs-lookup"><span data-stu-id="1ba8f-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ba8f-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ba8f-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1ba8f-173">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-173">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Assigned Products,Team Chat Message Count,Private Chat Message Count,Call Count,Meeting Count,Has Other Action,Report Period
```

### <a name="json"></a><span data-ttu-id="1ba8f-174">JSON</span><span class="sxs-lookup"><span data-stu-id="1ba8f-174">JSON</span></span>

<span data-ttu-id="1ba8f-175">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-175">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1ba8f-176">请求</span><span class="sxs-lookup"><span data-stu-id="1ba8f-176">Request</span></span>

<span data-ttu-id="1ba8f-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-177">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1ba8f-178">响应</span><span class="sxs-lookup"><span data-stu-id="1ba8f-178">Response</span></span>

<span data-ttu-id="1ba8f-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-179">The following is an example of the response.</span></span>

> <span data-ttu-id="1ba8f-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1ba8f-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
      "teamChatMessageCount": 0, 
      "privateChatMessageCount": 49, 
      "callCount": 2, 
      "meetingCount": 0, 
      "hasOtherAction": true, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1ba8f-182">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1ba8f-182">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1ba8f-183">语言</span><span class="sxs-lookup"><span data-stu-id="1ba8f-183">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1ba8f-184">Javascript</span><span class="sxs-lookup"><span data-stu-id="1ba8f-184">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getteamsuseractivityuserdetail_json-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getteamsuseractivityuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
