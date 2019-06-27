---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2f1ed658cc0234c12e472b87438cafeee2e4d7ad
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267240"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="eb8e6-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="eb8e6-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb8e6-105">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="eb8e6-106">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="eb8e6-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb8e6-108">权限</span><span class="sxs-lookup"><span data-stu-id="eb8e6-108">Permissions</span></span>

<span data-ttu-id="eb8e6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="eb8e6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb8e6-111">Permission type</span></span>                        | <span data-ttu-id="eb8e6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eb8e6-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="eb8e6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb8e6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="eb8e6-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb8e6-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="eb8e6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb8e6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb8e6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-116">Not supported.</span></span>                           |
| <span data-ttu-id="eb8e6-117">应用</span><span class="sxs-lookup"><span data-stu-id="eb8e6-117">Application</span></span>                            | <span data-ttu-id="eb8e6-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="eb8e6-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="eb8e6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb8e6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="eb8e6-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="eb8e6-120">Function parameters</span></span>

<span data-ttu-id="eb8e6-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="eb8e6-122">参数</span><span class="sxs-lookup"><span data-stu-id="eb8e6-122">Parameter</span></span> | <span data-ttu-id="eb8e6-123">类型</span><span class="sxs-lookup"><span data-stu-id="eb8e6-123">Type</span></span>   | <span data-ttu-id="eb8e6-124">说明</span><span class="sxs-lookup"><span data-stu-id="eb8e6-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="eb8e6-125">period</span><span class="sxs-lookup"><span data-stu-id="eb8e6-125">period</span></span>    | <span data-ttu-id="eb8e6-126">string</span><span class="sxs-lookup"><span data-stu-id="eb8e6-126">string</span></span> | <span data-ttu-id="eb8e6-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="eb8e6-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="eb8e6-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="eb8e6-130">必需。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-130">Required.</span></span> |

<span data-ttu-id="eb8e6-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="eb8e6-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-132">The default output type is text/csv.</span></span> <span data-ttu-id="eb8e6-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="eb8e6-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb8e6-134">Request headers</span></span>

| <span data-ttu-id="eb8e6-135">名称</span><span class="sxs-lookup"><span data-stu-id="eb8e6-135">Name</span></span>          | <span data-ttu-id="eb8e6-136">说明</span><span class="sxs-lookup"><span data-stu-id="eb8e6-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="eb8e6-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb8e6-137">Authorization</span></span> | <span data-ttu-id="eb8e6-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="eb8e6-140">响应</span><span class="sxs-lookup"><span data-stu-id="eb8e6-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="eb8e6-141">CSV</span><span class="sxs-lookup"><span data-stu-id="eb8e6-141">CSV</span></span>

<span data-ttu-id="eb8e6-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="eb8e6-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="eb8e6-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="eb8e6-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="eb8e6-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="eb8e6-146">Report Refresh Date</span></span>
- <span data-ttu-id="eb8e6-147">网站类型</span><span class="sxs-lookup"><span data-stu-id="eb8e6-147">Site Type</span></span>
- <span data-ttu-id="eb8e6-148">总计</span><span class="sxs-lookup"><span data-stu-id="eb8e6-148">Total</span></span>
- <span data-ttu-id="eb8e6-149">活跃</span><span class="sxs-lookup"><span data-stu-id="eb8e6-149">Active</span></span>
- <span data-ttu-id="eb8e6-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="eb8e6-150">Report Date</span></span>
- <span data-ttu-id="eb8e6-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="eb8e6-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="eb8e6-152">JSON</span><span class="sxs-lookup"><span data-stu-id="eb8e6-152">JSON</span></span>

<span data-ttu-id="eb8e6-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-153">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eb8e6-154">示例</span><span class="sxs-lookup"><span data-stu-id="eb8e6-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="eb8e6-155">CSV</span><span class="sxs-lookup"><span data-stu-id="eb8e6-155">CSV</span></span>

<span data-ttu-id="eb8e6-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="eb8e6-157">请求</span><span class="sxs-lookup"><span data-stu-id="eb8e6-157">Request</span></span>

<span data-ttu-id="eb8e6-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="eb8e6-159">响应</span><span class="sxs-lookup"><span data-stu-id="eb8e6-159">Response</span></span>

<span data-ttu-id="eb8e6-160">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-160">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb8e6-161">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eb8e6-161">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb8e6-162">C#</span><span class="sxs-lookup"><span data-stu-id="eb8e6-162">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb8e6-163">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb8e6-163">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb8e6-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="eb8e6-164">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="eb8e6-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Site Type,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="eb8e6-166">JSON</span><span class="sxs-lookup"><span data-stu-id="eb8e6-166">JSON</span></span>

<span data-ttu-id="eb8e6-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="eb8e6-168">请求</span><span class="sxs-lookup"><span data-stu-id="eb8e6-168">Request</span></span>

<span data-ttu-id="eb8e6-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-169">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="eb8e6-170">响应</span><span class="sxs-lookup"><span data-stu-id="eb8e6-170">Response</span></span>

<span data-ttu-id="eb8e6-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-171">The following is an example of the response.</span></span>

> <span data-ttu-id="eb8e6-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="eb8e6-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="eb8e6-174">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="eb8e6-174">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="eb8e6-175">C#</span><span class="sxs-lookup"><span data-stu-id="eb8e6-175">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb8e6-176">Javascript</span><span class="sxs-lookup"><span data-stu-id="eb8e6-176">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="eb8e6-177">目标-C</span><span class="sxs-lookup"><span data-stu-id="eb8e6-177">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getsharepointsiteusagefilecounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getsharepointsiteusagefilecounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
