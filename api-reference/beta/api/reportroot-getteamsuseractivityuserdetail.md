---
title: 'reportRoot: getTeamsUserActivityUserDetail'
description: 按用户获取有关 Microsoft Teams 用户活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f931c31c2ba580af67f076b1761c518d0a5516cf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867083"
---
# <a name="reportroot-getteamsuseractivityuserdetail"></a><span data-ttu-id="6b105-103">reportRoot：getTeamsUserActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="6b105-103">reportRoot: getTeamsUserActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b105-104">按用户获取有关 Microsoft Teams 用户活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="6b105-104">Get details about Microsoft Teams user activity by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="6b105-105">权限</span><span class="sxs-lookup"><span data-stu-id="6b105-105">Permissions</span></span>

<span data-ttu-id="6b105-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6b105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6b105-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b105-108">Permission type</span></span>                        | <span data-ttu-id="6b105-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b105-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="6b105-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b105-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6b105-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b105-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="6b105-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b105-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b105-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b105-113">Not supported.</span></span>                           |
| <span data-ttu-id="6b105-114">应用</span><span class="sxs-lookup"><span data-stu-id="6b105-114">Application</span></span>                            | <span data-ttu-id="6b105-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b105-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="6b105-116">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="6b105-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="6b105-117">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="6b105-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="6b105-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b105-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsUserActivityUserDetail(period='D7')
GET /reports/getTeamsUserActivityUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="6b105-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="6b105-119">Function parameters</span></span>

<span data-ttu-id="6b105-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="6b105-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="6b105-121">参数</span><span class="sxs-lookup"><span data-stu-id="6b105-121">Parameter</span></span> | <span data-ttu-id="6b105-122">类型</span><span class="sxs-lookup"><span data-stu-id="6b105-122">Type</span></span>   | <span data-ttu-id="6b105-123">说明</span><span class="sxs-lookup"><span data-stu-id="6b105-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="6b105-124">period</span><span class="sxs-lookup"><span data-stu-id="6b105-124">period</span></span>    | <span data-ttu-id="6b105-125">string</span><span class="sxs-lookup"><span data-stu-id="6b105-125">string</span></span> | <span data-ttu-id="6b105-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6b105-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="6b105-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="6b105-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="6b105-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="6b105-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="6b105-129">date</span><span class="sxs-lookup"><span data-stu-id="6b105-129">date</span></span>      | <span data-ttu-id="6b105-130">Date</span><span class="sxs-lookup"><span data-stu-id="6b105-130">Date</span></span>   | <span data-ttu-id="6b105-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="6b105-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="6b105-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="6b105-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="6b105-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="6b105-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="6b105-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="6b105-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="6b105-135">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6b105-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="6b105-136">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="6b105-136">The default output type is text/csv.</span></span> <span data-ttu-id="6b105-137">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="6b105-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6b105-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b105-138">Request headers</span></span>

| <span data-ttu-id="6b105-139">名称</span><span class="sxs-lookup"><span data-stu-id="6b105-139">Name</span></span>          | <span data-ttu-id="6b105-140">说明</span><span class="sxs-lookup"><span data-stu-id="6b105-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="6b105-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b105-141">Authorization</span></span> | <span data-ttu-id="6b105-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6b105-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="6b105-144">响应</span><span class="sxs-lookup"><span data-stu-id="6b105-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="6b105-145">CSV</span><span class="sxs-lookup"><span data-stu-id="6b105-145">CSV</span></span>

<span data-ttu-id="6b105-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="6b105-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="6b105-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="6b105-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="6b105-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="6b105-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="6b105-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="6b105-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="6b105-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="6b105-150">Report Refresh Date</span></span>
- <span data-ttu-id="6b105-151">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="6b105-151">User Principal Name</span></span>
- <span data-ttu-id="6b105-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="6b105-152">Last Activity Date</span></span>
- <span data-ttu-id="6b105-153">已删除</span><span class="sxs-lookup"><span data-stu-id="6b105-153">Is Deleted</span></span>
- <span data-ttu-id="6b105-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="6b105-154">Deleted Date</span></span>
- <span data-ttu-id="6b105-155">分配的产品</span><span class="sxs-lookup"><span data-stu-id="6b105-155">Assigned Products</span></span>
- <span data-ttu-id="6b105-156">团队聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="6b105-156">Team Chat Message Count</span></span>
- <span data-ttu-id="6b105-157">专用聊天消息计数</span><span class="sxs-lookup"><span data-stu-id="6b105-157">Private Chat Message Count</span></span>
- <span data-ttu-id="6b105-158">呼叫计数</span><span class="sxs-lookup"><span data-stu-id="6b105-158">Call Count</span></span>
- <span data-ttu-id="6b105-159">会议计数</span><span class="sxs-lookup"><span data-stu-id="6b105-159">Meeting Count</span></span>
- <span data-ttu-id="6b105-160">包含其他操作</span><span class="sxs-lookup"><span data-stu-id="6b105-160">Has Other Action</span></span>
- <span data-ttu-id="6b105-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="6b105-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="6b105-162">JSON</span><span class="sxs-lookup"><span data-stu-id="6b105-162">JSON</span></span>

<span data-ttu-id="6b105-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="6b105-163">If successful, this method returns a `200 OK` response code and a **[teamsUserActivityUserDetail](../resources/teamsuseractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="6b105-164">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="6b105-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="6b105-165">示例</span><span class="sxs-lookup"><span data-stu-id="6b105-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="6b105-166">CSV</span><span class="sxs-lookup"><span data-stu-id="6b105-166">CSV</span></span>

<span data-ttu-id="6b105-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="6b105-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="6b105-168">请求</span><span class="sxs-lookup"><span data-stu-id="6b105-168">Request</span></span>

<span data-ttu-id="6b105-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b105-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b105-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b105-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b105-171">C#</span><span class="sxs-lookup"><span data-stu-id="6b105-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b105-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b105-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b105-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b105-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6b105-174">响应</span><span class="sxs-lookup"><span data-stu-id="6b105-174">Response</span></span>

<span data-ttu-id="6b105-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6b105-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="6b105-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="6b105-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="6b105-177">JSON</span><span class="sxs-lookup"><span data-stu-id="6b105-177">JSON</span></span>

<span data-ttu-id="6b105-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="6b105-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="6b105-179">请求</span><span class="sxs-lookup"><span data-stu-id="6b105-179">Request</span></span>

<span data-ttu-id="6b105-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6b105-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="6b105-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="6b105-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsuseractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsUserActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6b105-182">C#</span><span class="sxs-lookup"><span data-stu-id="6b105-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsuseractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6b105-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6b105-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsuseractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6b105-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6b105-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsuseractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6b105-185">响应</span><span class="sxs-lookup"><span data-stu-id="6b105-185">Response</span></span>

<span data-ttu-id="6b105-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="6b105-186">The following is an example of the response.</span></span>

> <span data-ttu-id="6b105-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6b105-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
