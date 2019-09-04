---
title: 'reportRoot: getYammerGroupsActivityCounts'
description: 获取组中已发布、已阅读和已赞的 Yammer 消息数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 461811f13dd49ce6241538a4aea21f75a668b90c
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724825"
---
# <a name="reportroot-getyammergroupsactivitycounts"></a><span data-ttu-id="dfd1a-103">reportRoot: getYammerGroupsActivityCounts</span><span class="sxs-lookup"><span data-stu-id="dfd1a-103">reportRoot: getYammerGroupsActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dfd1a-104">获取组中已发布、已阅读和已赞的 Yammer 消息数。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-104">Get the number of Yammer messages posted, read, and liked in groups.</span></span>

> <span data-ttu-id="dfd1a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfd1a-106">权限</span><span class="sxs-lookup"><span data-stu-id="dfd1a-106">Permissions</span></span>

<span data-ttu-id="dfd1a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dfd1a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfd1a-109">Permission type</span></span>                        | <span data-ttu-id="dfd1a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfd1a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="dfd1a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd1a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dfd1a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfd1a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="dfd1a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfd1a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfd1a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-114">Not supported.</span></span>                           |
| <span data-ttu-id="dfd1a-115">应用</span><span class="sxs-lookup"><span data-stu-id="dfd1a-115">Application</span></span>                            | <span data-ttu-id="dfd1a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfd1a-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="dfd1a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfd1a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="dfd1a-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="dfd1a-118">Function parameters</span></span>

<span data-ttu-id="dfd1a-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="dfd1a-120">参数</span><span class="sxs-lookup"><span data-stu-id="dfd1a-120">Parameter</span></span> | <span data-ttu-id="dfd1a-121">类型</span><span class="sxs-lookup"><span data-stu-id="dfd1a-121">Type</span></span>   | <span data-ttu-id="dfd1a-122">说明</span><span class="sxs-lookup"><span data-stu-id="dfd1a-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="dfd1a-123">period</span><span class="sxs-lookup"><span data-stu-id="dfd1a-123">period</span></span>    | <span data-ttu-id="dfd1a-124">string</span><span class="sxs-lookup"><span data-stu-id="dfd1a-124">string</span></span> | <span data-ttu-id="dfd1a-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="dfd1a-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="dfd1a-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="dfd1a-128">必需。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-128">Required.</span></span> |

<span data-ttu-id="dfd1a-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="dfd1a-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-130">The default output type is text/csv.</span></span> <span data-ttu-id="dfd1a-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dfd1a-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfd1a-132">Request headers</span></span>

| <span data-ttu-id="dfd1a-133">名称</span><span class="sxs-lookup"><span data-stu-id="dfd1a-133">Name</span></span>          | <span data-ttu-id="dfd1a-134">说明</span><span class="sxs-lookup"><span data-stu-id="dfd1a-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="dfd1a-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfd1a-135">Authorization</span></span> | <span data-ttu-id="dfd1a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="dfd1a-138">响应</span><span class="sxs-lookup"><span data-stu-id="dfd1a-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="dfd1a-139">CSV</span><span class="sxs-lookup"><span data-stu-id="dfd1a-139">CSV</span></span>

<span data-ttu-id="dfd1a-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="dfd1a-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="dfd1a-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="dfd1a-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="dfd1a-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="dfd1a-144">Report Refresh Date</span></span>
- <span data-ttu-id="dfd1a-145">已赞</span><span class="sxs-lookup"><span data-stu-id="dfd1a-145">Liked</span></span>
- <span data-ttu-id="dfd1a-146">已发布</span><span class="sxs-lookup"><span data-stu-id="dfd1a-146">Posted</span></span>
- <span data-ttu-id="dfd1a-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="dfd1a-147">Read</span></span>
- <span data-ttu-id="dfd1a-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="dfd1a-148">Report Date</span></span>
- <span data-ttu-id="dfd1a-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="dfd1a-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="dfd1a-150">JSON</span><span class="sxs-lookup"><span data-stu-id="dfd1a-150">JSON</span></span>

<span data-ttu-id="dfd1a-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-151">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityCounts](../resources/yammergroupsactivitycounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfd1a-152">示例</span><span class="sxs-lookup"><span data-stu-id="dfd1a-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="dfd1a-153">CSV</span><span class="sxs-lookup"><span data-stu-id="dfd1a-153">CSV</span></span>

<span data-ttu-id="dfd1a-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="dfd1a-155">请求</span><span class="sxs-lookup"><span data-stu-id="dfd1a-155">Request</span></span>

<span data-ttu-id="dfd1a-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-156">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dfd1a-157">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dfd1a-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfd1a-158">C#</span><span class="sxs-lookup"><span data-stu-id="dfd1a-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfd1a-159">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd1a-159">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfd1a-160">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfd1a-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfd1a-161">响应</span><span class="sxs-lookup"><span data-stu-id="dfd1a-161">Response</span></span>

<span data-ttu-id="dfd1a-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-162">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="dfd1a-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Liked,Posted,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="dfd1a-164">JSON</span><span class="sxs-lookup"><span data-stu-id="dfd1a-164">JSON</span></span>

<span data-ttu-id="dfd1a-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="dfd1a-166">请求</span><span class="sxs-lookup"><span data-stu-id="dfd1a-166">Request</span></span>

<span data-ttu-id="dfd1a-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dfd1a-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="dfd1a-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dfd1a-169">C#</span><span class="sxs-lookup"><span data-stu-id="dfd1a-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dfd1a-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfd1a-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dfd1a-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="dfd1a-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="dfd1a-172">响应</span><span class="sxs-lookup"><span data-stu-id="dfd1a-172">Response</span></span>

<span data-ttu-id="dfd1a-173">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-173">The following is an example of the response.</span></span>

> <span data-ttu-id="dfd1a-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dfd1a-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerGroupsActivityCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 241

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerGroupsActivityCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 13, 
      "posted": 50, 
      "read": 69, 
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
