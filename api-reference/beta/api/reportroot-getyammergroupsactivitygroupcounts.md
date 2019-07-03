---
title: 'reportRoot: getYammerGroupsActivityGroupCounts'
description: 获取存在的总组数，以及有多少组包含组对话活动。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 7c6762deb54f96d22f60bd0c8511ddcb94a375d1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446309"
---
# <a name="reportroot-getyammergroupsactivitygroupcounts"></a><span data-ttu-id="0b3fc-103">reportRoot: getYammerGroupsActivityGroupCounts</span><span class="sxs-lookup"><span data-stu-id="0b3fc-103">reportRoot: getYammerGroupsActivityGroupCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b3fc-104">获取存在的总组数，以及有多少组包含组对话活动。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-104">Get the total number of groups that existed and how many included group conversation activity.</span></span>

> <span data-ttu-id="0b3fc-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 组活动](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31)。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer groups activity](https://support.office.com/client/Yammer-groups-activity-report-94dd92ec-ea73-43c6-b51f-2a11fd78aa31).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b3fc-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b3fc-106">Permissions</span></span>

<span data-ttu-id="0b3fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b3fc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b3fc-109">Permission type</span></span>                        | <span data-ttu-id="0b3fc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b3fc-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b3fc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b3fc-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b3fc-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b3fc-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b3fc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b3fc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b3fc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b3fc-115">应用</span><span class="sxs-lookup"><span data-stu-id="0b3fc-115">Application</span></span>                            | <span data-ttu-id="0b3fc-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b3fc-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="0b3fc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b3fc-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerGroupsActivityGroupCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0b3fc-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="0b3fc-118">Function parameters</span></span>

<span data-ttu-id="0b3fc-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0b3fc-120">参数</span><span class="sxs-lookup"><span data-stu-id="0b3fc-120">Parameter</span></span> | <span data-ttu-id="0b3fc-121">类型</span><span class="sxs-lookup"><span data-stu-id="0b3fc-121">Type</span></span>   | <span data-ttu-id="0b3fc-122">说明</span><span class="sxs-lookup"><span data-stu-id="0b3fc-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b3fc-123">period</span><span class="sxs-lookup"><span data-stu-id="0b3fc-123">period</span></span>    | <span data-ttu-id="0b3fc-124">string</span><span class="sxs-lookup"><span data-stu-id="0b3fc-124">string</span></span> | <span data-ttu-id="0b3fc-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b3fc-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b3fc-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0b3fc-128">必需。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-128">Required.</span></span> |

<span data-ttu-id="0b3fc-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0b3fc-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-130">The default output type is text/csv.</span></span> <span data-ttu-id="0b3fc-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b3fc-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b3fc-132">Request headers</span></span>

| <span data-ttu-id="0b3fc-133">名称</span><span class="sxs-lookup"><span data-stu-id="0b3fc-133">Name</span></span>          | <span data-ttu-id="0b3fc-134">说明</span><span class="sxs-lookup"><span data-stu-id="0b3fc-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0b3fc-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b3fc-135">Authorization</span></span> | <span data-ttu-id="0b3fc-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0b3fc-138">响应</span><span class="sxs-lookup"><span data-stu-id="0b3fc-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0b3fc-139">CSV</span><span class="sxs-lookup"><span data-stu-id="0b3fc-139">CSV</span></span>

<span data-ttu-id="0b3fc-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b3fc-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b3fc-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b3fc-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="0b3fc-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0b3fc-144">Report Refresh Date</span></span>
- <span data-ttu-id="0b3fc-145">总计</span><span class="sxs-lookup"><span data-stu-id="0b3fc-145">Total</span></span>
- <span data-ttu-id="0b3fc-146">活跃</span><span class="sxs-lookup"><span data-stu-id="0b3fc-146">Active</span></span>
- <span data-ttu-id="0b3fc-147">报表日期</span><span class="sxs-lookup"><span data-stu-id="0b3fc-147">Report Date</span></span>
- <span data-ttu-id="0b3fc-148">报表周期</span><span class="sxs-lookup"><span data-stu-id="0b3fc-148">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="0b3fc-149">JSON</span><span class="sxs-lookup"><span data-stu-id="0b3fc-149">JSON</span></span>

<span data-ttu-id="0b3fc-150">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-150">If successful, this method returns a `200 OK` response code and a **[yammerGroupsActivityGroupCounts](../resources/yammergroupsactivitygroupcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b3fc-151">示例</span><span class="sxs-lookup"><span data-stu-id="0b3fc-151">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0b3fc-152">CSV</span><span class="sxs-lookup"><span data-stu-id="0b3fc-152">CSV</span></span>

<span data-ttu-id="0b3fc-153">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-153">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0b3fc-154">请求</span><span class="sxs-lookup"><span data-stu-id="0b3fc-154">Request</span></span>

<span data-ttu-id="0b3fc-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-155">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b3fc-156">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0b3fc-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b3fc-157">C#</span><span class="sxs-lookup"><span data-stu-id="0b3fc-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b3fc-158">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b3fc-158">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b3fc-159">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b3fc-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b3fc-160">响应</span><span class="sxs-lookup"><span data-stu-id="0b3fc-160">Response</span></span>

<span data-ttu-id="0b3fc-161">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-161">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b3fc-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="0b3fc-163">JSON</span><span class="sxs-lookup"><span data-stu-id="0b3fc-163">JSON</span></span>

<span data-ttu-id="0b3fc-164">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0b3fc-165">请求</span><span class="sxs-lookup"><span data-stu-id="0b3fc-165">Request</span></span>

<span data-ttu-id="0b3fc-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-166">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b3fc-167">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="0b3fc-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammergroupsactivitygroupcounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerGroupsActivityGroupCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b3fc-168">C#</span><span class="sxs-lookup"><span data-stu-id="0b3fc-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammergroupsactivitygroupcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b3fc-169">Javascript</span><span class="sxs-lookup"><span data-stu-id="0b3fc-169">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammergroupsactivitygroupcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b3fc-170">目标-C</span><span class="sxs-lookup"><span data-stu-id="0b3fc-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammergroupsactivitygroupcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b3fc-171">响应</span><span class="sxs-lookup"><span data-stu-id="0b3fc-171">Response</span></span>

<span data-ttu-id="0b3fc-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-172">The following is an example of the response.</span></span>

> <span data-ttu-id="0b3fc-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0b3fc-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
