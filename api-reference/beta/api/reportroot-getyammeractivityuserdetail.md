---
title: 'reportRoot: getYammerActivityUserDetail'
description: 获取用户执行的 Yammer 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 9a541aa570fac81d5410250e9ea167a7ccfd427b
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724867"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="57c9c-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="57c9c-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="57c9c-104">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="57c9c-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="57c9c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="57c9c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="57c9c-106">权限</span><span class="sxs-lookup"><span data-stu-id="57c9c-106">Permissions</span></span>

<span data-ttu-id="57c9c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57c9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="57c9c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="57c9c-109">Permission type</span></span>                        | <span data-ttu-id="57c9c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57c9c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="57c9c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57c9c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="57c9c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c9c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="57c9c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57c9c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="57c9c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="57c9c-114">Not supported.</span></span>                           |
| <span data-ttu-id="57c9c-115">应用</span><span class="sxs-lookup"><span data-stu-id="57c9c-115">Application</span></span>                            | <span data-ttu-id="57c9c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="57c9c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="57c9c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57c9c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="57c9c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="57c9c-118">Function parameters</span></span>

<span data-ttu-id="57c9c-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="57c9c-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="57c9c-120">参数</span><span class="sxs-lookup"><span data-stu-id="57c9c-120">Parameter</span></span> | <span data-ttu-id="57c9c-121">类型</span><span class="sxs-lookup"><span data-stu-id="57c9c-121">Type</span></span>   | <span data-ttu-id="57c9c-122">说明</span><span class="sxs-lookup"><span data-stu-id="57c9c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="57c9c-123">period</span><span class="sxs-lookup"><span data-stu-id="57c9c-123">period</span></span>    | <span data-ttu-id="57c9c-124">string</span><span class="sxs-lookup"><span data-stu-id="57c9c-124">string</span></span> | <span data-ttu-id="57c9c-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="57c9c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="57c9c-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="57c9c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="57c9c-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="57c9c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="57c9c-128">date</span><span class="sxs-lookup"><span data-stu-id="57c9c-128">date</span></span>      | <span data-ttu-id="57c9c-129">Date</span><span class="sxs-lookup"><span data-stu-id="57c9c-129">Date</span></span>   | <span data-ttu-id="57c9c-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="57c9c-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="57c9c-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="57c9c-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="57c9c-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="57c9c-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="57c9c-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="57c9c-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="57c9c-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="57c9c-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="57c9c-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="57c9c-135">The default output type is text/csv.</span></span> <span data-ttu-id="57c9c-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="57c9c-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="57c9c-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="57c9c-137">Request headers</span></span>

| <span data-ttu-id="57c9c-138">名称</span><span class="sxs-lookup"><span data-stu-id="57c9c-138">Name</span></span>          | <span data-ttu-id="57c9c-139">说明</span><span class="sxs-lookup"><span data-stu-id="57c9c-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="57c9c-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="57c9c-140">Authorization</span></span> | <span data-ttu-id="57c9c-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="57c9c-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="57c9c-143">响应</span><span class="sxs-lookup"><span data-stu-id="57c9c-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="57c9c-144">CSV</span><span class="sxs-lookup"><span data-stu-id="57c9c-144">CSV</span></span>

<span data-ttu-id="57c9c-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="57c9c-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="57c9c-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="57c9c-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="57c9c-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="57c9c-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="57c9c-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="57c9c-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="57c9c-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="57c9c-149">Report Refresh Date</span></span>
- <span data-ttu-id="57c9c-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="57c9c-150">User Principal Name</span></span>
- <span data-ttu-id="57c9c-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="57c9c-151">Display Name</span></span>
- <span data-ttu-id="57c9c-152">用户状态</span><span class="sxs-lookup"><span data-stu-id="57c9c-152">User State</span></span>
- <span data-ttu-id="57c9c-153">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="57c9c-153">State Change Date</span></span>
- <span data-ttu-id="57c9c-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="57c9c-154">Last Activity Date</span></span>
- <span data-ttu-id="57c9c-155">已发布数</span><span class="sxs-lookup"><span data-stu-id="57c9c-155">Posted Count</span></span>
- <span data-ttu-id="57c9c-156">已阅读数</span><span class="sxs-lookup"><span data-stu-id="57c9c-156">Read Count</span></span>
- <span data-ttu-id="57c9c-157">已赞数</span><span class="sxs-lookup"><span data-stu-id="57c9c-157">Liked Count</span></span>
- <span data-ttu-id="57c9c-158">分配的产品</span><span class="sxs-lookup"><span data-stu-id="57c9c-158">Assigned Products</span></span>
- <span data-ttu-id="57c9c-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="57c9c-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="57c9c-160">JSON</span><span class="sxs-lookup"><span data-stu-id="57c9c-160">JSON</span></span>

<span data-ttu-id="57c9c-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="57c9c-161">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="57c9c-162">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="57c9c-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="57c9c-163">示例</span><span class="sxs-lookup"><span data-stu-id="57c9c-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="57c9c-164">CSV</span><span class="sxs-lookup"><span data-stu-id="57c9c-164">CSV</span></span>

<span data-ttu-id="57c9c-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="57c9c-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="57c9c-166">请求</span><span class="sxs-lookup"><span data-stu-id="57c9c-166">Request</span></span>

<span data-ttu-id="57c9c-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57c9c-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="57c9c-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="57c9c-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57c9c-169">C#</span><span class="sxs-lookup"><span data-stu-id="57c9c-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57c9c-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57c9c-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57c9c-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="57c9c-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57c9c-172">响应</span><span class="sxs-lookup"><span data-stu-id="57c9c-172">Response</span></span>

<span data-ttu-id="57c9c-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="57c9c-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="57c9c-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="57c9c-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Posted Count,Read Count,Liked Count,Assigned Products,Report Period
```

### <a name="json"></a><span data-ttu-id="57c9c-175">JSON</span><span class="sxs-lookup"><span data-stu-id="57c9c-175">JSON</span></span>

<span data-ttu-id="57c9c-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="57c9c-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="57c9c-177">请求</span><span class="sxs-lookup"><span data-stu-id="57c9c-177">Request</span></span>

<span data-ttu-id="57c9c-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="57c9c-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="57c9c-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="57c9c-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="57c9c-180">C#</span><span class="sxs-lookup"><span data-stu-id="57c9c-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="57c9c-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="57c9c-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="57c9c-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="57c9c-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="57c9c-183">响应</span><span class="sxs-lookup"><span data-stu-id="57c9c-183">Response</span></span>

<span data-ttu-id="57c9c-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="57c9c-184">The following is an example of the response.</span></span>

> <span data-ttu-id="57c9c-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="57c9c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivityUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 434

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivityUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2015-08-26", 
      "lastActivityDate": "2017-09-01", 
      "postedCount": 2, 
      "readCount": 5, 
      "likedCount": 0, 
      "assignedProducts": [
        "OFFICE 365 ENTERPRISE E5"
      ], 
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
