---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 0e5928b3d131a53e85f4560a98cdc00e222a5a29
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267319"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="c2dab-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="c2dab-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2dab-104">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c2dab-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="c2dab-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="c2dab-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="c2dab-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2dab-106">Permissions</span></span>

<span data-ttu-id="c2dab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2dab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2dab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2dab-109">Permission type</span></span>                        | <span data-ttu-id="c2dab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2dab-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c2dab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2dab-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2dab-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2dab-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c2dab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2dab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2dab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2dab-114">Not supported.</span></span>                           |
| <span data-ttu-id="c2dab-115">应用</span><span class="sxs-lookup"><span data-stu-id="c2dab-115">Application</span></span>                            | <span data-ttu-id="c2dab-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c2dab-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c2dab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2dab-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="c2dab-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="c2dab-118">Function parameters</span></span>

<span data-ttu-id="c2dab-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c2dab-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c2dab-120">参数</span><span class="sxs-lookup"><span data-stu-id="c2dab-120">Parameter</span></span> | <span data-ttu-id="c2dab-121">类型</span><span class="sxs-lookup"><span data-stu-id="c2dab-121">Type</span></span>   | <span data-ttu-id="c2dab-122">说明</span><span class="sxs-lookup"><span data-stu-id="c2dab-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c2dab-123">period</span><span class="sxs-lookup"><span data-stu-id="c2dab-123">period</span></span>    | <span data-ttu-id="c2dab-124">string</span><span class="sxs-lookup"><span data-stu-id="c2dab-124">string</span></span> | <span data-ttu-id="c2dab-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c2dab-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c2dab-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c2dab-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c2dab-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c2dab-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c2dab-128">date</span><span class="sxs-lookup"><span data-stu-id="c2dab-128">date</span></span>      | <span data-ttu-id="c2dab-129">Date</span><span class="sxs-lookup"><span data-stu-id="c2dab-129">Date</span></span>   | <span data-ttu-id="c2dab-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="c2dab-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c2dab-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="c2dab-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c2dab-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="c2dab-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c2dab-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="c2dab-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c2dab-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c2dab-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c2dab-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="c2dab-135">The default output type is text/csv.</span></span> <span data-ttu-id="c2dab-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="c2dab-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c2dab-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2dab-137">Request headers</span></span>

| <span data-ttu-id="c2dab-138">名称</span><span class="sxs-lookup"><span data-stu-id="c2dab-138">Name</span></span>          | <span data-ttu-id="c2dab-139">说明</span><span class="sxs-lookup"><span data-stu-id="c2dab-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c2dab-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2dab-140">Authorization</span></span> | <span data-ttu-id="c2dab-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2dab-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c2dab-143">响应</span><span class="sxs-lookup"><span data-stu-id="c2dab-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c2dab-144">CSV</span><span class="sxs-lookup"><span data-stu-id="c2dab-144">CSV</span></span>

<span data-ttu-id="c2dab-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c2dab-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c2dab-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c2dab-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c2dab-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="c2dab-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c2dab-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="c2dab-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c2dab-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c2dab-149">Report Refresh Date</span></span>
- <span data-ttu-id="c2dab-150">网站 URL</span><span class="sxs-lookup"><span data-stu-id="c2dab-150">Site URL</span></span>
- <span data-ttu-id="c2dab-151">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="c2dab-151">Owner Display Name</span></span>
- <span data-ttu-id="c2dab-152">已删除</span><span class="sxs-lookup"><span data-stu-id="c2dab-152">Is Deleted</span></span>
- <span data-ttu-id="c2dab-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="c2dab-153">Last Activity Date</span></span>
- <span data-ttu-id="c2dab-154">文件数</span><span class="sxs-lookup"><span data-stu-id="c2dab-154">File Count</span></span>
- <span data-ttu-id="c2dab-155">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="c2dab-155">Active File Count</span></span>
- <span data-ttu-id="c2dab-156">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="c2dab-156">Storage Used (Byte)</span></span>
- <span data-ttu-id="c2dab-157">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="c2dab-157">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="c2dab-158">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="c2dab-158">Owner Principal Name</span></span>
- <span data-ttu-id="c2dab-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="c2dab-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c2dab-160">JSON</span><span class="sxs-lookup"><span data-stu-id="c2dab-160">JSON</span></span>

<span data-ttu-id="c2dab-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="c2dab-161">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c2dab-162">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="c2dab-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="c2dab-163">示例</span><span class="sxs-lookup"><span data-stu-id="c2dab-163">Example</span></span>

<span data-ttu-id="c2dab-164">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2dab-164">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="c2dab-165">CSV</span><span class="sxs-lookup"><span data-stu-id="c2dab-165">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="c2dab-166">请求</span><span class="sxs-lookup"><span data-stu-id="c2dab-166">Request</span></span>

<span data-ttu-id="c2dab-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2dab-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="c2dab-168">响应</span><span class="sxs-lookup"><span data-stu-id="c2dab-168">Response</span></span>

<span data-ttu-id="c2dab-169">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c2dab-169">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2dab-170">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c2dab-170">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2dab-171">C#</span><span class="sxs-lookup"><span data-stu-id="c2dab-171">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2dab-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2dab-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2dab-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2dab-173">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="c2dab-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c2dab-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site URL,Owner Display Name,Is Deleted,Last Activity Date,File Count,Active File Count,Storage Used (Byte),Storage Allocated (Byte),Owner Principal Name,Report Period
```

### <a name="json"></a><span data-ttu-id="c2dab-175">JSON</span><span class="sxs-lookup"><span data-stu-id="c2dab-175">JSON</span></span>

<span data-ttu-id="c2dab-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="c2dab-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c2dab-177">请求</span><span class="sxs-lookup"><span data-stu-id="c2dab-177">Request</span></span>

<span data-ttu-id="c2dab-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c2dab-178">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="c2dab-179">响应</span><span class="sxs-lookup"><span data-stu-id="c2dab-179">Response</span></span>

<span data-ttu-id="c2dab-180">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c2dab-180">The following is an example of the response.</span></span>

> <span data-ttu-id="c2dab-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c2dab-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 400

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteUrl": "siteUrl-value", 
      "ownerDisplayName": "ownerDisplayName-value", 
      "ownerPrincipalName": "ownerPrincipalName-value", 
      "isDeleted": false, 
      "lastActivityDate": "2017-09-01", 
      "fileCount": 9, 
      "activeFileCount": 5, 
      "storageUsedInBytes": 12190375, 
      "storageAllocatedInBytes": 549755813880, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="c2dab-183">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c2dab-183">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c2dab-184">C#</span><span class="sxs-lookup"><span data-stu-id="c2dab-184">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2dab-185">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2dab-185">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c2dab-186">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2dab-186">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getonedriveusageaccountdetail_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getonedriveusageaccountdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
