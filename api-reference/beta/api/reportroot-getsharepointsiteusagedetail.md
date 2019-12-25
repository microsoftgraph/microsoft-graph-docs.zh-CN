---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: 获取 SharePoint 网站使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: aa1ce1a704a02504795a45ea6c7ac7f6c9879762
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867433"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="3bc10-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="3bc10-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bc10-104">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3bc10-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="3bc10-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="3bc10-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="3bc10-106">权限</span><span class="sxs-lookup"><span data-stu-id="3bc10-106">Permissions</span></span>

<span data-ttu-id="3bc10-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3bc10-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3bc10-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3bc10-109">Permission type</span></span>                        | <span data-ttu-id="3bc10-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3bc10-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3bc10-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3bc10-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3bc10-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bc10-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3bc10-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3bc10-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3bc10-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3bc10-114">Not supported.</span></span>                           |
| <span data-ttu-id="3bc10-115">应用</span><span class="sxs-lookup"><span data-stu-id="3bc10-115">Application</span></span>                            | <span data-ttu-id="3bc10-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3bc10-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3bc10-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3bc10-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3bc10-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3bc10-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3bc10-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3bc10-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3bc10-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="3bc10-120">Function parameters</span></span>

<span data-ttu-id="3bc10-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3bc10-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3bc10-122">参数</span><span class="sxs-lookup"><span data-stu-id="3bc10-122">Parameter</span></span> | <span data-ttu-id="3bc10-123">类型</span><span class="sxs-lookup"><span data-stu-id="3bc10-123">Type</span></span>   | <span data-ttu-id="3bc10-124">说明</span><span class="sxs-lookup"><span data-stu-id="3bc10-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3bc10-125">period</span><span class="sxs-lookup"><span data-stu-id="3bc10-125">period</span></span>    | <span data-ttu-id="3bc10-126">string</span><span class="sxs-lookup"><span data-stu-id="3bc10-126">string</span></span> | <span data-ttu-id="3bc10-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3bc10-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3bc10-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3bc10-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3bc10-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3bc10-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3bc10-130">date</span><span class="sxs-lookup"><span data-stu-id="3bc10-130">date</span></span>      | <span data-ttu-id="3bc10-131">Date</span><span class="sxs-lookup"><span data-stu-id="3bc10-131">Date</span></span>   | <span data-ttu-id="3bc10-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="3bc10-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3bc10-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="3bc10-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3bc10-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="3bc10-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3bc10-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="3bc10-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3bc10-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3bc10-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3bc10-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3bc10-137">The default output type is text/csv.</span></span> <span data-ttu-id="3bc10-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3bc10-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3bc10-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="3bc10-139">Request headers</span></span>

| <span data-ttu-id="3bc10-140">名称</span><span class="sxs-lookup"><span data-stu-id="3bc10-140">Name</span></span>          | <span data-ttu-id="3bc10-141">说明</span><span class="sxs-lookup"><span data-stu-id="3bc10-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3bc10-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="3bc10-142">Authorization</span></span> | <span data-ttu-id="3bc10-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3bc10-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3bc10-145">响应</span><span class="sxs-lookup"><span data-stu-id="3bc10-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3bc10-146">CSV</span><span class="sxs-lookup"><span data-stu-id="3bc10-146">CSV</span></span>

<span data-ttu-id="3bc10-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3bc10-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3bc10-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3bc10-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3bc10-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="3bc10-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3bc10-150">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="3bc10-150">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3bc10-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3bc10-151">Report Refresh Date</span></span>
- <span data-ttu-id="3bc10-152">网站 Id</span><span class="sxs-lookup"><span data-stu-id="3bc10-152">Site Id</span></span>
- <span data-ttu-id="3bc10-153">网站 URL</span><span class="sxs-lookup"><span data-stu-id="3bc10-153">Site URL</span></span>
- <span data-ttu-id="3bc10-154">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="3bc10-154">Owner Display Name</span></span>
- <span data-ttu-id="3bc10-155">已删除</span><span class="sxs-lookup"><span data-stu-id="3bc10-155">Is Deleted</span></span>
- <span data-ttu-id="3bc10-156">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3bc10-156">Last Activity Date</span></span>
- <span data-ttu-id="3bc10-157">文件数</span><span class="sxs-lookup"><span data-stu-id="3bc10-157">File Count</span></span>
- <span data-ttu-id="3bc10-158">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="3bc10-158">Active File Count</span></span>
- <span data-ttu-id="3bc10-159">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="3bc10-159">Page View Count</span></span>
- <span data-ttu-id="3bc10-160">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="3bc10-160">Visited Page Count</span></span>
- <span data-ttu-id="3bc10-161">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="3bc10-161">Storage Used (Byte)</span></span>
- <span data-ttu-id="3bc10-162">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="3bc10-162">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="3bc10-163">根网站模板</span><span class="sxs-lookup"><span data-stu-id="3bc10-163">Root Web Template</span></span>
- <span data-ttu-id="3bc10-164">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="3bc10-164">Owner Principal Name</span></span>
- <span data-ttu-id="3bc10-165">报表周期</span><span class="sxs-lookup"><span data-stu-id="3bc10-165">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3bc10-166">JSON</span><span class="sxs-lookup"><span data-stu-id="3bc10-166">JSON</span></span>

<span data-ttu-id="3bc10-167">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3bc10-167">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="3bc10-168">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="3bc10-168">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3bc10-169">示例</span><span class="sxs-lookup"><span data-stu-id="3bc10-169">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3bc10-170">CSV</span><span class="sxs-lookup"><span data-stu-id="3bc10-170">CSV</span></span>

<span data-ttu-id="3bc10-171">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3bc10-171">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3bc10-172">请求</span><span class="sxs-lookup"><span data-stu-id="3bc10-172">Request</span></span>

<span data-ttu-id="3bc10-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3bc10-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3bc10-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc10-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3bc10-175">C#</span><span class="sxs-lookup"><span data-stu-id="3bc10-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc10-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bc10-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3bc10-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bc10-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3bc10-178">响应</span><span class="sxs-lookup"><span data-stu-id="3bc10-178">Response</span></span>

<span data-ttu-id="3bc10-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3bc10-179">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3bc10-180">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3bc10-180">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Id,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Page View Count,Visited Page Count,Storage Used (Byte),Storage Allocated (Byte),Root Web Template,Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="3bc10-181">JSON</span><span class="sxs-lookup"><span data-stu-id="3bc10-181">JSON</span></span>

<span data-ttu-id="3bc10-182">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3bc10-182">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3bc10-183">请求</span><span class="sxs-lookup"><span data-stu-id="3bc10-183">Request</span></span>

<span data-ttu-id="3bc10-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3bc10-184">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3bc10-185">HTTP</span><span class="sxs-lookup"><span data-stu-id="3bc10-185">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3bc10-186">C#</span><span class="sxs-lookup"><span data-stu-id="3bc10-186">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3bc10-187">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3bc10-187">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3bc10-188">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3bc10-188">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3bc10-189">响应</span><span class="sxs-lookup"><span data-stu-id="3bc10-189">Response</span></span>

<span data-ttu-id="3bc10-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3bc10-190">The following is an example of the response.</span></span>

> <span data-ttu-id="3bc10-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3bc10-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 484

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteId": "siteId-value", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 170, 
      "activeFileCount": 25, 
      "pageViewCount": 7, 
      "visitedPageCount": 3, 
      "storageUsedInBytes": 63442116, 
      "storageAllocatedInBytes": 2748779094400, 
      "rootWebTemplate": "Publishing Site", 
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
