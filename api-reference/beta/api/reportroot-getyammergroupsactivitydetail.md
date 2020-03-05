---
title: 'reportRoot: getYammerGroupsActivityDetail'
description: 获取组执行的 Yammer 组活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 0f24445dc38edbdab501ca0212fd1ee1c4575e0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453952"
---
# <a name="reportroot-getyammergroupsactivitydetail"></a><span data-ttu-id="a06bf-103">reportRoot: getYammerGroupsActivityDetail</span><span class="sxs-lookup"><span data-stu-id="a06bf-103">reportRoot: getYammerGroupsActivityDetail</span></span>

<span data-ttu-id="a06bf-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a06bf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a06bf-105">获取组执行的 Yammer 组活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="a06bf-105">Get details about Yammer groups activity by group.</span></span>

> <span data-ttu-id="a06bf-106">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="a06bf-106">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="a06bf-107">权限</span><span class="sxs-lookup"><span data-stu-id="a06bf-107">Permissions</span></span>

<span data-ttu-id="a06bf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a06bf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a06bf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a06bf-110">Permission type</span></span>                        | <span data-ttu-id="a06bf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a06bf-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a06bf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a06bf-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="a06bf-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a06bf-113">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a06bf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a06bf-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a06bf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a06bf-115">Not supported.</span></span>                           |
| <span data-ttu-id="a06bf-116">应用</span><span class="sxs-lookup"><span data-stu-id="a06bf-116">Application</span></span>                            | <span data-ttu-id="a06bf-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a06bf-117">Reports.Read.All</span></span>                         |

<span data-ttu-id="a06bf-118">**注意**：若要获得委派权限以允许应用代表用户读取服务使用情况报告，租户管理员必须事先为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a06bf-118">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a06bf-119">有关更多详细信息，请参阅 [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a06bf-119">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a06bf-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a06bf-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityDetail(period='{period_value}')
GET /reports/getYammerGroupsActivityDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="a06bf-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="a06bf-121">Function parameters</span></span>

<span data-ttu-id="a06bf-122">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a06bf-122">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="a06bf-123">参数</span><span class="sxs-lookup"><span data-stu-id="a06bf-123">Parameter</span></span> | <span data-ttu-id="a06bf-124">类型</span><span class="sxs-lookup"><span data-stu-id="a06bf-124">Type</span></span>   | <span data-ttu-id="a06bf-125">说明</span><span class="sxs-lookup"><span data-stu-id="a06bf-125">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a06bf-126">period</span><span class="sxs-lookup"><span data-stu-id="a06bf-126">period</span></span>    | <span data-ttu-id="a06bf-127">string</span><span class="sxs-lookup"><span data-stu-id="a06bf-127">string</span></span> | <span data-ttu-id="a06bf-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a06bf-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a06bf-129">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a06bf-129">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a06bf-130">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a06bf-130">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="a06bf-131">date</span><span class="sxs-lookup"><span data-stu-id="a06bf-131">date</span></span>      | <span data-ttu-id="a06bf-132">Date</span><span class="sxs-lookup"><span data-stu-id="a06bf-132">Date</span></span>   | <span data-ttu-id="a06bf-133">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="a06bf-133">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="a06bf-134">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="a06bf-134">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="a06bf-135">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="a06bf-135">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="a06bf-136">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="a06bf-136">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="a06bf-137">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a06bf-137">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a06bf-138">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a06bf-138">The default output type is text/csv.</span></span> <span data-ttu-id="a06bf-139">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a06bf-139">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a06bf-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="a06bf-140">Request headers</span></span>

| <span data-ttu-id="a06bf-141">名称</span><span class="sxs-lookup"><span data-stu-id="a06bf-141">Name</span></span>          | <span data-ttu-id="a06bf-142">说明</span><span class="sxs-lookup"><span data-stu-id="a06bf-142">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a06bf-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="a06bf-143">Authorization</span></span> | <span data-ttu-id="a06bf-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a06bf-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a06bf-146">响应</span><span class="sxs-lookup"><span data-stu-id="a06bf-146">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a06bf-147">CSV</span><span class="sxs-lookup"><span data-stu-id="a06bf-147">CSV</span></span>

<span data-ttu-id="a06bf-148">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a06bf-148">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a06bf-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a06bf-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a06bf-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a06bf-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a06bf-151">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a06bf-151">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a06bf-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a06bf-152">Report Refresh Date</span></span>
- <span data-ttu-id="a06bf-153">组显示名称</span><span class="sxs-lookup"><span data-stu-id="a06bf-153">Group Display Name</span></span>
- <span data-ttu-id="a06bf-154">已删除</span><span class="sxs-lookup"><span data-stu-id="a06bf-154">Is Deleted</span></span>
- <span data-ttu-id="a06bf-155">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="a06bf-155">Owner Principal Name</span></span>
- <span data-ttu-id="a06bf-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="a06bf-156">Last Activity Date</span></span>
- <span data-ttu-id="a06bf-157">组类型</span><span class="sxs-lookup"><span data-stu-id="a06bf-157">Group Type</span></span>
- <span data-ttu-id="a06bf-158">Office 365 已连接</span><span class="sxs-lookup"><span data-stu-id="a06bf-158">Office 365 Connected</span></span>
- <span data-ttu-id="a06bf-159">成员数</span><span class="sxs-lookup"><span data-stu-id="a06bf-159">Member Count</span></span>
- <span data-ttu-id="a06bf-160">已发布数</span><span class="sxs-lookup"><span data-stu-id="a06bf-160">Posted Count</span></span>
- <span data-ttu-id="a06bf-161">已阅读数</span><span class="sxs-lookup"><span data-stu-id="a06bf-161">Read Count</span></span>
- <span data-ttu-id="a06bf-162">已赞数</span><span class="sxs-lookup"><span data-stu-id="a06bf-162">Liked Count</span></span>
- <span data-ttu-id="a06bf-163">报表周期</span><span class="sxs-lookup"><span data-stu-id="a06bf-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a06bf-164">JSON</span><span class="sxs-lookup"><span data-stu-id="a06bf-164">JSON</span></span>

<span data-ttu-id="a06bf-165">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a06bf-165">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityDetail](../resources/yammergroupsactivitydetail.md)** object in the response body.</span></span>

<span data-ttu-id="a06bf-166">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="a06bf-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="a06bf-167">示例</span><span class="sxs-lookup"><span data-stu-id="a06bf-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a06bf-168">CSV</span><span class="sxs-lookup"><span data-stu-id="a06bf-168">CSV</span></span>

<span data-ttu-id="a06bf-169">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a06bf-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a06bf-170">请求</span><span class="sxs-lookup"><span data-stu-id="a06bf-170">Request</span></span>

<span data-ttu-id="a06bf-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a06bf-171">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a06bf-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a06bf-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="a06bf-173">C#</span><span class="sxs-lookup"><span data-stu-id="a06bf-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a06bf-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a06bf-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a06bf-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a06bf-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a06bf-176">响应</span><span class="sxs-lookup"><span data-stu-id="a06bf-176">Response</span></span>

<span data-ttu-id="a06bf-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a06bf-177">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a06bf-178">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a06bf-178">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Group Display Name,Is Deleted,Owner Principal Name,Last Activity Date,Group Type,Office 365 Connected,Member Count,Posted Count,Read Count,Liked Count,Report Period
```

### <a name="json"></a><span data-ttu-id="a06bf-179">JSON</span><span class="sxs-lookup"><span data-stu-id="a06bf-179">JSON</span></span>

<span data-ttu-id="a06bf-180">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a06bf-180">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a06bf-181">请求</span><span class="sxs-lookup"><span data-stu-id="a06bf-181">Request</span></span>

<span data-ttu-id="a06bf-182">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a06bf-182">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="a06bf-183">HTTP</span><span class="sxs-lookup"><span data-stu-id="a06bf-183">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitydetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityDetail(period='D7')?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="a06bf-184">C#</span><span class="sxs-lookup"><span data-stu-id="a06bf-184">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitydetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a06bf-185">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a06bf-185">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitydetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a06bf-186">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a06bf-186">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitydetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a06bf-187">响应</span><span class="sxs-lookup"><span data-stu-id="a06bf-187">Response</span></span>

<span data-ttu-id="a06bf-188">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a06bf-188">The following is an example of the response.</span></span>

> <span data-ttu-id="a06bf-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a06bf-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 441

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "groupDisplayName": "groupDisplayName-value", 
      "isDeleted": false, 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "lastActivityDate": "2017-08-30", 
      "groupType": "private", 
      "office365Connected": true, 
      "memberCount": 176, 
      "postedCount": 15, 
      "readCount": 24, 
      "likedCount": 3, 
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
