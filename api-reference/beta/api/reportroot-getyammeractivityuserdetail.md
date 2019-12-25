---
title: 'reportRoot: getYammerActivityUserDetail'
description: 获取用户执行的 Yammer 活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 45c5439aee587345e2505010e60b9be0414282f1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868890"
---
# <a name="reportroot-getyammeractivityuserdetail"></a><span data-ttu-id="19e92-103">reportRoot: getYammerActivityUserDetail</span><span class="sxs-lookup"><span data-stu-id="19e92-103">reportRoot: getYammerActivityUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19e92-104">获取用户执行的 Yammer 活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="19e92-104">Get details about Yammer activity by user.</span></span>

> <span data-ttu-id="19e92-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="19e92-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="19e92-106">权限</span><span class="sxs-lookup"><span data-stu-id="19e92-106">Permissions</span></span>

<span data-ttu-id="19e92-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19e92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="19e92-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19e92-109">Permission type</span></span>                        | <span data-ttu-id="19e92-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19e92-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="19e92-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19e92-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="19e92-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19e92-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="19e92-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19e92-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19e92-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="19e92-114">Not supported.</span></span>                           |
| <span data-ttu-id="19e92-115">应用</span><span class="sxs-lookup"><span data-stu-id="19e92-115">Application</span></span>                            | <span data-ttu-id="19e92-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="19e92-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="19e92-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="19e92-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="19e92-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="19e92-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="19e92-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19e92-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserDetail(period='{period_value}')
GET /reports/getYammerActivityUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="19e92-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="19e92-120">Function parameters</span></span>

<span data-ttu-id="19e92-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="19e92-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="19e92-122">参数</span><span class="sxs-lookup"><span data-stu-id="19e92-122">Parameter</span></span> | <span data-ttu-id="19e92-123">类型</span><span class="sxs-lookup"><span data-stu-id="19e92-123">Type</span></span>   | <span data-ttu-id="19e92-124">说明</span><span class="sxs-lookup"><span data-stu-id="19e92-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="19e92-125">period</span><span class="sxs-lookup"><span data-stu-id="19e92-125">period</span></span>    | <span data-ttu-id="19e92-126">string</span><span class="sxs-lookup"><span data-stu-id="19e92-126">string</span></span> | <span data-ttu-id="19e92-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="19e92-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="19e92-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="19e92-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="19e92-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="19e92-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="19e92-130">date</span><span class="sxs-lookup"><span data-stu-id="19e92-130">date</span></span>      | <span data-ttu-id="19e92-131">Date</span><span class="sxs-lookup"><span data-stu-id="19e92-131">Date</span></span>   | <span data-ttu-id="19e92-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="19e92-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="19e92-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="19e92-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="19e92-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="19e92-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="19e92-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="19e92-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="19e92-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19e92-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="19e92-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="19e92-137">The default output type is text/csv.</span></span> <span data-ttu-id="19e92-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="19e92-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="19e92-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="19e92-139">Request headers</span></span>

| <span data-ttu-id="19e92-140">名称</span><span class="sxs-lookup"><span data-stu-id="19e92-140">Name</span></span>          | <span data-ttu-id="19e92-141">说明</span><span class="sxs-lookup"><span data-stu-id="19e92-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="19e92-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="19e92-142">Authorization</span></span> | <span data-ttu-id="19e92-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19e92-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="19e92-145">响应</span><span class="sxs-lookup"><span data-stu-id="19e92-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="19e92-146">CSV</span><span class="sxs-lookup"><span data-stu-id="19e92-146">CSV</span></span>

<span data-ttu-id="19e92-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="19e92-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="19e92-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="19e92-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="19e92-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="19e92-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="19e92-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="19e92-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="19e92-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="19e92-151">Report Refresh Date</span></span>
- <span data-ttu-id="19e92-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="19e92-152">User Principal Name</span></span>
- <span data-ttu-id="19e92-153">显示名称</span><span class="sxs-lookup"><span data-stu-id="19e92-153">Display Name</span></span>
- <span data-ttu-id="19e92-154">用户状态</span><span class="sxs-lookup"><span data-stu-id="19e92-154">User State</span></span>
- <span data-ttu-id="19e92-155">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="19e92-155">State Change Date</span></span>
- <span data-ttu-id="19e92-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="19e92-156">Last Activity Date</span></span>
- <span data-ttu-id="19e92-157">已发布数</span><span class="sxs-lookup"><span data-stu-id="19e92-157">Posted Count</span></span>
- <span data-ttu-id="19e92-158">已阅读数</span><span class="sxs-lookup"><span data-stu-id="19e92-158">Read Count</span></span>
- <span data-ttu-id="19e92-159">已赞数</span><span class="sxs-lookup"><span data-stu-id="19e92-159">Liked Count</span></span>
- <span data-ttu-id="19e92-160">分配的产品</span><span class="sxs-lookup"><span data-stu-id="19e92-160">Assigned Products</span></span>
- <span data-ttu-id="19e92-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="19e92-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="19e92-162">JSON</span><span class="sxs-lookup"><span data-stu-id="19e92-162">JSON</span></span>

<span data-ttu-id="19e92-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="19e92-163">If successful, this method returns a `200 OK` response code and a **[yammerActivityUserDetail](../resources/yammeractivityuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="19e92-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="19e92-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="19e92-165">示例</span><span class="sxs-lookup"><span data-stu-id="19e92-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="19e92-166">CSV</span><span class="sxs-lookup"><span data-stu-id="19e92-166">CSV</span></span>

<span data-ttu-id="19e92-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="19e92-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="19e92-168">请求</span><span class="sxs-lookup"><span data-stu-id="19e92-168">Request</span></span>

<span data-ttu-id="19e92-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19e92-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19e92-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e92-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19e92-171">C#</span><span class="sxs-lookup"><span data-stu-id="19e92-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19e92-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19e92-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19e92-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19e92-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19e92-174">响应</span><span class="sxs-lookup"><span data-stu-id="19e92-174">Response</span></span>

<span data-ttu-id="19e92-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="19e92-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="19e92-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="19e92-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="19e92-177">JSON</span><span class="sxs-lookup"><span data-stu-id="19e92-177">JSON</span></span>

<span data-ttu-id="19e92-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="19e92-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="19e92-179">请求</span><span class="sxs-lookup"><span data-stu-id="19e92-179">Request</span></span>

<span data-ttu-id="19e92-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="19e92-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="19e92-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="19e92-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="19e92-182">C#</span><span class="sxs-lookup"><span data-stu-id="19e92-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="19e92-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="19e92-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="19e92-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="19e92-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="19e92-185">响应</span><span class="sxs-lookup"><span data-stu-id="19e92-185">Response</span></span>

<span data-ttu-id="19e92-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="19e92-186">The following is an example of the response.</span></span>

> <span data-ttu-id="19e92-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="19e92-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
