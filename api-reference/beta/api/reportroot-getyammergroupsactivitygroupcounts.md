---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: 获取存在的总组数，以及有多少组包含组对话活动。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 1e8ee29729efef5dfcf0bda0a9404934f34d61cb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267086"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="65955-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="65955-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65955-104">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="65955-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="65955-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="65955-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="65955-106">权限</span><span class="sxs-lookup"><span data-stu-id="65955-106">Permissions</span></span>

<span data-ttu-id="65955-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65955-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="65955-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="65955-109">Permission type</span></span>                        | <span data-ttu-id="65955-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65955-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="65955-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65955-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="65955-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65955-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="65955-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65955-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65955-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="65955-114">Not supported.</span></span>                           |
| <span data-ttu-id="65955-115">应用</span><span class="sxs-lookup"><span data-stu-id="65955-115">Application</span></span>                            | <span data-ttu-id="65955-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="65955-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="65955-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65955-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="65955-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="65955-118">Function parameters</span></span>

<span data-ttu-id="65955-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="65955-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="65955-120">参数</span><span class="sxs-lookup"><span data-stu-id="65955-120">Parameter</span></span> | <span data-ttu-id="65955-121">类型</span><span class="sxs-lookup"><span data-stu-id="65955-121">Type</span></span>   | <span data-ttu-id="65955-122">说明</span><span class="sxs-lookup"><span data-stu-id="65955-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="65955-123">period</span><span class="sxs-lookup"><span data-stu-id="65955-123">period</span></span>    | <span data-ttu-id="65955-124">string</span><span class="sxs-lookup"><span data-stu-id="65955-124">string</span></span> | <span data-ttu-id="65955-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="65955-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="65955-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="65955-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="65955-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="65955-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="65955-128">必需。</span><span class="sxs-lookup"><span data-stu-id="65955-128">Required.</span></span> |

<span data-ttu-id="65955-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="65955-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="65955-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="65955-130">The default output type is text/csv.</span></span> <span data-ttu-id="65955-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="65955-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65955-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="65955-132">Request headers</span></span>

| <span data-ttu-id="65955-133">名称</span><span class="sxs-lookup"><span data-stu-id="65955-133">Name</span></span>          | <span data-ttu-id="65955-134">说明</span><span class="sxs-lookup"><span data-stu-id="65955-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="65955-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="65955-135">Authorization</span></span> | <span data-ttu-id="65955-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65955-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="65955-138">响应</span><span class="sxs-lookup"><span data-stu-id="65955-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="65955-139">CSV</span><span class="sxs-lookup"><span data-stu-id="65955-139">CSV</span></span>

<span data-ttu-id="65955-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="65955-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="65955-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="65955-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="65955-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="65955-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="65955-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="65955-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="65955-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="65955-144">Report Refresh Date</span></span>
- <span data-ttu-id="65955-145">总计</span><span class="sxs-lookup"><span data-stu-id="65955-145">Total</span></span>
- <span data-ttu-id="65955-146">活跃</span><span class="sxs-lookup"><span data-stu-id="65955-146">Active</span></span>
- <span data-ttu-id="65955-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="65955-147">Report Date</span></span>
- <span data-ttu-id="65955-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="65955-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="65955-149">JSON</span><span class="sxs-lookup"><span data-stu-id="65955-149">JSON</span></span>

<span data-ttu-id="65955-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="65955-150">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65955-151">示例</span><span class="sxs-lookup"><span data-stu-id="65955-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="65955-152">CSV</span><span class="sxs-lookup"><span data-stu-id="65955-152">CSV</span></span>

<span data-ttu-id="65955-153">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="65955-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="65955-154">请求</span><span class="sxs-lookup"><span data-stu-id="65955-154">Request</span></span>

<span data-ttu-id="65955-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="65955-155">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="65955-156">响应</span><span class="sxs-lookup"><span data-stu-id="65955-156">Response</span></span>

<span data-ttu-id="65955-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="65955-157">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="65955-158">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="65955-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65955-159">C#</span><span class="sxs-lookup"><span data-stu-id="65955-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65955-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="65955-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65955-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="65955-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="65955-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="65955-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Total,Active,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="65955-163">JSON</span><span class="sxs-lookup"><span data-stu-id="65955-163">JSON</span></span>

<span data-ttu-id="65955-164">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="65955-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="65955-165">请求</span><span class="sxs-lookup"><span data-stu-id="65955-165">Request</span></span>

<span data-ttu-id="65955-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="65955-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="65955-167">响应</span><span class="sxs-lookup"><span data-stu-id="65955-167">Response</span></span>

<span data-ttu-id="65955-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="65955-168">The following is an example of the response.</span></span>

> <span data-ttu-id="65955-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="65955-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityGroupCounts",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityGroupCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01",
      "total": 50, 
      "active": 41, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="65955-171">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="65955-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="65955-172">C#</span><span class="sxs-lookup"><span data-stu-id="65955-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65955-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="65955-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="65955-174">目标-C</span><span class="sxs-lookup"><span data-stu-id="65955-174">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getyammergroupsactivitygroupcounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammergroupsactivitygroupcounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
