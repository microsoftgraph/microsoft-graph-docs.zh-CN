---
title: 'reportRoot: getYammerActivityUserCounts'
description: 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 45d308c037d69fc845a0ede7289bfdfa0f322328
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639080"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="1fffa-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="1fffa-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1fffa-104">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="1fffa-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="1fffa-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="1fffa-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="1fffa-106">权限</span><span class="sxs-lookup"><span data-stu-id="1fffa-106">Permissions</span></span>

<span data-ttu-id="1fffa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1fffa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1fffa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1fffa-109">Permission type</span></span>                        | <span data-ttu-id="1fffa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1fffa-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="1fffa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1fffa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1fffa-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fffa-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="1fffa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1fffa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1fffa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1fffa-114">Not supported.</span></span>                           |
| <span data-ttu-id="1fffa-115">应用</span><span class="sxs-lookup"><span data-stu-id="1fffa-115">Application</span></span>                            | <span data-ttu-id="1fffa-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="1fffa-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="1fffa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1fffa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="1fffa-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="1fffa-118">Function parameters</span></span>

<span data-ttu-id="1fffa-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="1fffa-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="1fffa-120">参数</span><span class="sxs-lookup"><span data-stu-id="1fffa-120">Parameter</span></span> | <span data-ttu-id="1fffa-121">类型</span><span class="sxs-lookup"><span data-stu-id="1fffa-121">Type</span></span>   | <span data-ttu-id="1fffa-122">说明</span><span class="sxs-lookup"><span data-stu-id="1fffa-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="1fffa-123">period</span><span class="sxs-lookup"><span data-stu-id="1fffa-123">period</span></span>    | <span data-ttu-id="1fffa-124">string</span><span class="sxs-lookup"><span data-stu-id="1fffa-124">string</span></span> | <span data-ttu-id="1fffa-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1fffa-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="1fffa-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="1fffa-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="1fffa-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="1fffa-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="1fffa-128">必需。</span><span class="sxs-lookup"><span data-stu-id="1fffa-128">Required.</span></span> |

<span data-ttu-id="1fffa-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1fffa-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="1fffa-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="1fffa-130">The default output type is text/csv.</span></span> <span data-ttu-id="1fffa-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="1fffa-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1fffa-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="1fffa-132">Request headers</span></span>

| <span data-ttu-id="1fffa-133">名称</span><span class="sxs-lookup"><span data-stu-id="1fffa-133">Name</span></span>          | <span data-ttu-id="1fffa-134">说明</span><span class="sxs-lookup"><span data-stu-id="1fffa-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="1fffa-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="1fffa-135">Authorization</span></span> | <span data-ttu-id="1fffa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1fffa-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="1fffa-138">响应</span><span class="sxs-lookup"><span data-stu-id="1fffa-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="1fffa-139">CSV</span><span class="sxs-lookup"><span data-stu-id="1fffa-139">CSV</span></span>

<span data-ttu-id="1fffa-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="1fffa-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="1fffa-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="1fffa-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="1fffa-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="1fffa-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="1fffa-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="1fffa-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="1fffa-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="1fffa-144">Report Refresh Date</span></span>
- <span data-ttu-id="1fffa-145">已赞</span><span class="sxs-lookup"><span data-stu-id="1fffa-145">Liked</span></span>
- <span data-ttu-id="1fffa-146">已发布</span><span class="sxs-lookup"><span data-stu-id="1fffa-146">Posted</span></span>
- <span data-ttu-id="1fffa-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="1fffa-147">Read</span></span>
- <span data-ttu-id="1fffa-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="1fffa-148">Report Date</span></span>
- <span data-ttu-id="1fffa-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="1fffa-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="1fffa-150">JSON</span><span class="sxs-lookup"><span data-stu-id="1fffa-150">JSON</span></span>

<span data-ttu-id="1fffa-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="1fffa-151">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1fffa-152">示例</span><span class="sxs-lookup"><span data-stu-id="1fffa-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="1fffa-153">CSV</span><span class="sxs-lookup"><span data-stu-id="1fffa-153">CSV</span></span>

<span data-ttu-id="1fffa-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="1fffa-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="1fffa-155">请求</span><span class="sxs-lookup"><span data-stu-id="1fffa-155">Request</span></span>

<span data-ttu-id="1fffa-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1fffa-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="1fffa-157">响应</span><span class="sxs-lookup"><span data-stu-id="1fffa-157">Response</span></span>

<span data-ttu-id="1fffa-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1fffa-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1fffa-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1fffa-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1fffa-160">语言</span><span class="sxs-lookup"><span data-stu-id="1fffa-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fffa-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="1fffa-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_csv-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="1fffa-162">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="1fffa-162">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="1fffa-163">JSON</span><span class="sxs-lookup"><span data-stu-id="1fffa-163">JSON</span></span>

<span data-ttu-id="1fffa-164">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="1fffa-164">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="1fffa-165">请求</span><span class="sxs-lookup"><span data-stu-id="1fffa-165">Request</span></span>

<span data-ttu-id="1fffa-166">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="1fffa-166">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="1fffa-167">响应</span><span class="sxs-lookup"><span data-stu-id="1fffa-167">Response</span></span>

<span data-ttu-id="1fffa-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="1fffa-168">The following is an example of the response.</span></span>

> <span data-ttu-id="1fffa-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1fffa-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 236

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 40, 
      "posted": 54, 
      "read": 28, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="1fffa-171">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="1fffa-171">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1fffa-172">语言</span><span class="sxs-lookup"><span data-stu-id="1fffa-172">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1fffa-173">Javascript</span><span class="sxs-lookup"><span data-stu-id="1fffa-173">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getyammeractivityusercounts_json-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getyammeractivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
