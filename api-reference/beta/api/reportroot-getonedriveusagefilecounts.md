---
title: 'reportRoot: getOneDriveUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3c47f6ec97f55ceab0801dcc2893e92cd418b980
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411527"
---
# <a name="reportroot-getonedriveusagefilecounts"></a><span data-ttu-id="5e372-104">reportRoot: getOneDriveUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="5e372-104">reportRoot: getOneDriveUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e372-105">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="5e372-105">Get the total number of files across all sites and how many are active files.</span></span> <span data-ttu-id="5e372-106">如果文件在指定时间段内被保存、同步、修改或共享，则视为活跃文件。</span><span class="sxs-lookup"><span data-stu-id="5e372-106">A file is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="5e372-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="5e372-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e372-108">权限</span><span class="sxs-lookup"><span data-stu-id="5e372-108">Permissions</span></span>

<span data-ttu-id="5e372-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e372-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e372-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e372-111">Permission type</span></span>                        | <span data-ttu-id="5e372-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e372-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="5e372-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e372-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e372-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e372-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="5e372-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e372-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e372-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e372-116">Not supported.</span></span>                           |
| <span data-ttu-id="5e372-117">应用</span><span class="sxs-lookup"><span data-stu-id="5e372-117">Application</span></span>                            | <span data-ttu-id="5e372-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="5e372-118">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="5e372-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e372-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="5e372-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="5e372-120">Function parameters</span></span>

<span data-ttu-id="5e372-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="5e372-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="5e372-122">参数</span><span class="sxs-lookup"><span data-stu-id="5e372-122">Parameter</span></span> | <span data-ttu-id="5e372-123">类型</span><span class="sxs-lookup"><span data-stu-id="5e372-123">Type</span></span>   | <span data-ttu-id="5e372-124">说明</span><span class="sxs-lookup"><span data-stu-id="5e372-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="5e372-125">period</span><span class="sxs-lookup"><span data-stu-id="5e372-125">period</span></span>    | <span data-ttu-id="5e372-126">string</span><span class="sxs-lookup"><span data-stu-id="5e372-126">string</span></span> | <span data-ttu-id="5e372-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5e372-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="5e372-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="5e372-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="5e372-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="5e372-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="5e372-130">必需。</span><span class="sxs-lookup"><span data-stu-id="5e372-130">Required.</span></span> |

<span data-ttu-id="5e372-131">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5e372-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="5e372-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="5e372-132">The default output type is text/csv.</span></span> <span data-ttu-id="5e372-133">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="5e372-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5e372-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e372-134">Request headers</span></span>

| <span data-ttu-id="5e372-135">名称</span><span class="sxs-lookup"><span data-stu-id="5e372-135">Name</span></span>          | <span data-ttu-id="5e372-136">说明</span><span class="sxs-lookup"><span data-stu-id="5e372-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="5e372-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e372-137">Authorization</span></span> | <span data-ttu-id="5e372-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e372-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="5e372-140">响应</span><span class="sxs-lookup"><span data-stu-id="5e372-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="5e372-141">CSV</span><span class="sxs-lookup"><span data-stu-id="5e372-141">CSV</span></span>

<span data-ttu-id="5e372-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="5e372-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="5e372-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="5e372-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="5e372-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="5e372-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="5e372-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="5e372-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="5e372-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="5e372-146">Report Refresh Date</span></span>
- <span data-ttu-id="5e372-147">网站类型</span><span class="sxs-lookup"><span data-stu-id="5e372-147">Site Type</span></span>
- <span data-ttu-id="5e372-148">总计</span><span class="sxs-lookup"><span data-stu-id="5e372-148">Total</span></span>
- <span data-ttu-id="5e372-149">活跃</span><span class="sxs-lookup"><span data-stu-id="5e372-149">Active</span></span>
- <span data-ttu-id="5e372-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="5e372-150">Report Date</span></span>
- <span data-ttu-id="5e372-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="5e372-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="5e372-152">JSON</span><span class="sxs-lookup"><span data-stu-id="5e372-152">JSON</span></span>

<span data-ttu-id="5e372-153">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="5e372-153">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageFileCounts](../resources/onedriveusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e372-154">示例</span><span class="sxs-lookup"><span data-stu-id="5e372-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="5e372-155">CSV</span><span class="sxs-lookup"><span data-stu-id="5e372-155">CSV</span></span>

<span data-ttu-id="5e372-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="5e372-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="5e372-157">请求</span><span class="sxs-lookup"><span data-stu-id="5e372-157">Request</span></span>

<span data-ttu-id="5e372-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e372-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5e372-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5e372-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e372-160">C#</span><span class="sxs-lookup"><span data-stu-id="5e372-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e372-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e372-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e372-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="5e372-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e372-163">响应</span><span class="sxs-lookup"><span data-stu-id="5e372-163">Response</span></span>

<span data-ttu-id="5e372-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e372-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="5e372-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="5e372-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="5e372-166">JSON</span><span class="sxs-lookup"><span data-stu-id="5e372-166">JSON</span></span>

<span data-ttu-id="5e372-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="5e372-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="5e372-168">请求</span><span class="sxs-lookup"><span data-stu-id="5e372-168">Request</span></span>

<span data-ttu-id="5e372-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e372-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5e372-170">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="5e372-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusagefilecounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5e372-171">C#</span><span class="sxs-lookup"><span data-stu-id="5e372-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5e372-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e372-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5e372-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="5e372-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5e372-174">响应</span><span class="sxs-lookup"><span data-stu-id="5e372-174">Response</span></span>

<span data-ttu-id="5e372-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5e372-175">The following is an example of the response.</span></span>

> <span data-ttu-id="5e372-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5e372-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 251

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 297960, 
      "active": 4679, 
      "reportDate": "2017-09-01", 
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
