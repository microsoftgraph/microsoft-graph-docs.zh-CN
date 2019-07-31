---
title: 'reportRoot: getSharePointSiteUsageDetail'
description: 获取 SharePoint 网站使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c5de4ec3c1c54d2aa184bfb6bc9a2886905e4236
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991952"
---
# <a name="reportroot-getsharepointsiteusagedetail"></a><span data-ttu-id="3467d-103">reportRoot: getSharePointSiteUsageDetail</span><span class="sxs-lookup"><span data-stu-id="3467d-103">reportRoot: getSharePointSiteUsageDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3467d-104">获取 SharePoint 网站使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3467d-104">Get details about SharePoint site usage.</span></span>

> <span data-ttu-id="3467d-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="3467d-105">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="3467d-106">权限</span><span class="sxs-lookup"><span data-stu-id="3467d-106">Permissions</span></span>

<span data-ttu-id="3467d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3467d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3467d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3467d-109">Permission type</span></span>                        | <span data-ttu-id="3467d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3467d-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3467d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3467d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3467d-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3467d-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3467d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3467d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3467d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3467d-114">Not supported.</span></span>                           |
| <span data-ttu-id="3467d-115">应用</span><span class="sxs-lookup"><span data-stu-id="3467d-115">Application</span></span>                            | <span data-ttu-id="3467d-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3467d-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3467d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3467d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageDetail(period='{period_value}')
GET /reports/getSharePointSiteUsageDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3467d-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="3467d-118">Function parameters</span></span>

<span data-ttu-id="3467d-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3467d-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3467d-120">参数</span><span class="sxs-lookup"><span data-stu-id="3467d-120">Parameter</span></span> | <span data-ttu-id="3467d-121">类型</span><span class="sxs-lookup"><span data-stu-id="3467d-121">Type</span></span>   | <span data-ttu-id="3467d-122">说明</span><span class="sxs-lookup"><span data-stu-id="3467d-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3467d-123">period</span><span class="sxs-lookup"><span data-stu-id="3467d-123">period</span></span>    | <span data-ttu-id="3467d-124">string</span><span class="sxs-lookup"><span data-stu-id="3467d-124">string</span></span> | <span data-ttu-id="3467d-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3467d-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3467d-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3467d-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3467d-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3467d-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3467d-128">date</span><span class="sxs-lookup"><span data-stu-id="3467d-128">date</span></span>      | <span data-ttu-id="3467d-129">Date</span><span class="sxs-lookup"><span data-stu-id="3467d-129">Date</span></span>   | <span data-ttu-id="3467d-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="3467d-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3467d-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="3467d-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3467d-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="3467d-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3467d-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="3467d-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3467d-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3467d-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3467d-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3467d-135">The default output type is text/csv.</span></span> <span data-ttu-id="3467d-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3467d-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3467d-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="3467d-137">Request headers</span></span>

| <span data-ttu-id="3467d-138">名称</span><span class="sxs-lookup"><span data-stu-id="3467d-138">Name</span></span>          | <span data-ttu-id="3467d-139">说明</span><span class="sxs-lookup"><span data-stu-id="3467d-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3467d-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="3467d-140">Authorization</span></span> | <span data-ttu-id="3467d-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3467d-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3467d-143">响应</span><span class="sxs-lookup"><span data-stu-id="3467d-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3467d-144">CSV</span><span class="sxs-lookup"><span data-stu-id="3467d-144">CSV</span></span>

<span data-ttu-id="3467d-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3467d-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3467d-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3467d-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3467d-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="3467d-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3467d-148">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="3467d-148">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="3467d-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3467d-149">Report Refresh Date</span></span>
- <span data-ttu-id="3467d-150">网站 Id</span><span class="sxs-lookup"><span data-stu-id="3467d-150">Site Id</span></span>
- <span data-ttu-id="3467d-151">网站 URL</span><span class="sxs-lookup"><span data-stu-id="3467d-151">Site URL</span></span>
- <span data-ttu-id="3467d-152">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="3467d-152">Owner Display Name</span></span>
- <span data-ttu-id="3467d-153">已删除</span><span class="sxs-lookup"><span data-stu-id="3467d-153">Is Deleted</span></span>
- <span data-ttu-id="3467d-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3467d-154">Last Activity Date</span></span>
- <span data-ttu-id="3467d-155">文件数</span><span class="sxs-lookup"><span data-stu-id="3467d-155">File Count</span></span>
- <span data-ttu-id="3467d-156">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="3467d-156">Active File Count</span></span>
- <span data-ttu-id="3467d-157">页面浏览量</span><span class="sxs-lookup"><span data-stu-id="3467d-157">Page View Count</span></span>
- <span data-ttu-id="3467d-158">访问过的页面数</span><span class="sxs-lookup"><span data-stu-id="3467d-158">Visited Page Count</span></span>
- <span data-ttu-id="3467d-159">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="3467d-159">Storage Used (Byte)</span></span>
- <span data-ttu-id="3467d-160">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="3467d-160">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="3467d-161">根网站模板</span><span class="sxs-lookup"><span data-stu-id="3467d-161">Root Web Template</span></span>
- <span data-ttu-id="3467d-162">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="3467d-162">Owner Principal Name</span></span>
- <span data-ttu-id="3467d-163">报表周期</span><span class="sxs-lookup"><span data-stu-id="3467d-163">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3467d-164">JSON</span><span class="sxs-lookup"><span data-stu-id="3467d-164">JSON</span></span>

<span data-ttu-id="3467d-165">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3467d-165">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageDetail](../resources/sharepointsiteusagedetail.md)** object in the response body.</span></span>

<span data-ttu-id="3467d-166">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="3467d-166">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3467d-167">示例</span><span class="sxs-lookup"><span data-stu-id="3467d-167">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3467d-168">CSV</span><span class="sxs-lookup"><span data-stu-id="3467d-168">CSV</span></span>

<span data-ttu-id="3467d-169">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3467d-169">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3467d-170">请求</span><span class="sxs-lookup"><span data-stu-id="3467d-170">Request</span></span>

<span data-ttu-id="3467d-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3467d-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3467d-172">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3467d-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3467d-173">C#</span><span class="sxs-lookup"><span data-stu-id="3467d-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3467d-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="3467d-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3467d-175">目标-C</span><span class="sxs-lookup"><span data-stu-id="3467d-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3467d-176">Java</span><span class="sxs-lookup"><span data-stu-id="3467d-176">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3467d-177">响应</span><span class="sxs-lookup"><span data-stu-id="3467d-177">Response</span></span>

<span data-ttu-id="3467d-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3467d-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3467d-179">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3467d-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3467d-180">JSON</span><span class="sxs-lookup"><span data-stu-id="3467d-180">JSON</span></span>

<span data-ttu-id="3467d-181">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3467d-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3467d-182">请求</span><span class="sxs-lookup"><span data-stu-id="3467d-182">Request</span></span>

<span data-ttu-id="3467d-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3467d-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3467d-184">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3467d-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagedetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3467d-185">C#</span><span class="sxs-lookup"><span data-stu-id="3467d-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagedetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3467d-186">Javascript</span><span class="sxs-lookup"><span data-stu-id="3467d-186">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagedetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3467d-187">目标-C</span><span class="sxs-lookup"><span data-stu-id="3467d-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagedetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3467d-188">Java</span><span class="sxs-lookup"><span data-stu-id="3467d-188">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getsharepointsiteusagedetail-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3467d-189">响应</span><span class="sxs-lookup"><span data-stu-id="3467d-189">Response</span></span>

<span data-ttu-id="3467d-190">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3467d-190">The following is an example of the response.</span></span>

> <span data-ttu-id="3467d-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3467d-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
