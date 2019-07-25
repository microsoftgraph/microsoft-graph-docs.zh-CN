---
title: 'reportRoot: getOneDriveActivityUserCounts'
description: 获取 OneDrive 活跃用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 091b727af99eb71a383efc02d4b736b38f527994
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873108"
---
# <a name="reportroot-getonedriveactivityusercounts"></a><span data-ttu-id="161db-103">reportRoot: getOneDriveActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="161db-103">reportRoot: getOneDriveActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="161db-104">获取 OneDrive 活跃用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="161db-104">Get the trend in the number of active OneDrive users.</span></span>

> <span data-ttu-id="161db-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 活动](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353)。</span><span class="sxs-lookup"><span data-stu-id="161db-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business activity](https://support.office.com/client/OneDrive-for-Business-user-activity-8bbe4bf8-221b-46d6-99a5-2fb3c8ef9353).</span></span>

## <a name="permissions"></a><span data-ttu-id="161db-106">权限</span><span class="sxs-lookup"><span data-stu-id="161db-106">Permissions</span></span>

<span data-ttu-id="161db-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="161db-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="161db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="161db-109">Permission type</span></span>                        | <span data-ttu-id="161db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="161db-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="161db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="161db-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="161db-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="161db-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="161db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="161db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="161db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="161db-114">Not supported.</span></span>                           |
| <span data-ttu-id="161db-115">应用</span><span class="sxs-lookup"><span data-stu-id="161db-115">Application</span></span>                            | <span data-ttu-id="161db-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="161db-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="161db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="161db-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="161db-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="161db-118">Function parameters</span></span>

<span data-ttu-id="161db-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="161db-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="161db-120">参数</span><span class="sxs-lookup"><span data-stu-id="161db-120">Parameter</span></span> | <span data-ttu-id="161db-121">类型</span><span class="sxs-lookup"><span data-stu-id="161db-121">Type</span></span>   | <span data-ttu-id="161db-122">说明</span><span class="sxs-lookup"><span data-stu-id="161db-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="161db-123">period</span><span class="sxs-lookup"><span data-stu-id="161db-123">period</span></span>    | <span data-ttu-id="161db-124">string</span><span class="sxs-lookup"><span data-stu-id="161db-124">string</span></span> | <span data-ttu-id="161db-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="161db-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="161db-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="161db-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="161db-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="161db-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="161db-128">必需。</span><span class="sxs-lookup"><span data-stu-id="161db-128">Required.</span></span> |

<span data-ttu-id="161db-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="161db-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="161db-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="161db-130">The default output type is text/csv.</span></span> <span data-ttu-id="161db-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="161db-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="161db-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="161db-132">Request headers</span></span>

| <span data-ttu-id="161db-133">名称</span><span class="sxs-lookup"><span data-stu-id="161db-133">Name</span></span>          | <span data-ttu-id="161db-134">说明</span><span class="sxs-lookup"><span data-stu-id="161db-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="161db-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="161db-135">Authorization</span></span> | <span data-ttu-id="161db-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="161db-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="161db-138">响应</span><span class="sxs-lookup"><span data-stu-id="161db-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="161db-139">CSV</span><span class="sxs-lookup"><span data-stu-id="161db-139">CSV</span></span>

<span data-ttu-id="161db-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="161db-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="161db-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="161db-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="161db-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="161db-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="161db-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="161db-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="161db-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="161db-144">Report Refresh Date</span></span>
- <span data-ttu-id="161db-145">已查看或编辑</span><span class="sxs-lookup"><span data-stu-id="161db-145">Viewed Or Edited</span></span>
- <span data-ttu-id="161db-146">已同步</span><span class="sxs-lookup"><span data-stu-id="161db-146">Synced</span></span>
- <span data-ttu-id="161db-147">已内部共享</span><span class="sxs-lookup"><span data-stu-id="161db-147">Shared Internally</span></span>
- <span data-ttu-id="161db-148">已外部共享</span><span class="sxs-lookup"><span data-stu-id="161db-148">Shared Externally</span></span>
- <span data-ttu-id="161db-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="161db-149">Report Date</span></span>
- <span data-ttu-id="161db-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="161db-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="161db-151">JSON</span><span class="sxs-lookup"><span data-stu-id="161db-151">JSON</span></span>

<span data-ttu-id="161db-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[siteActivitySummary](../resources/siteactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="161db-152">If successful, this method returns a `200 OK` response code and a **[siteActivitySummary](../resources/siteactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="161db-153">示例</span><span class="sxs-lookup"><span data-stu-id="161db-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="161db-154">CSV</span><span class="sxs-lookup"><span data-stu-id="161db-154">CSV</span></span>

<span data-ttu-id="161db-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="161db-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="161db-156">请求</span><span class="sxs-lookup"><span data-stu-id="161db-156">Request</span></span>

<span data-ttu-id="161db-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="161db-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="161db-158">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="161db-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="161db-159">C#</span><span class="sxs-lookup"><span data-stu-id="161db-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="161db-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="161db-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="161db-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="161db-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="161db-162">Java</span><span class="sxs-lookup"><span data-stu-id="161db-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="161db-163">响应</span><span class="sxs-lookup"><span data-stu-id="161db-163">Response</span></span>

<span data-ttu-id="161db-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="161db-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="161db-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="161db-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Viewed Or Edited,Synced,Shared Internally,Shared Externally,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="161db-166">JSON</span><span class="sxs-lookup"><span data-stu-id="161db-166">JSON</span></span>

<span data-ttu-id="161db-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="161db-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="161db-168">请求</span><span class="sxs-lookup"><span data-stu-id="161db-168">Request</span></span>

<span data-ttu-id="161db-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="161db-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="161db-170">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="161db-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getOneDriveActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="161db-171">C#</span><span class="sxs-lookup"><span data-stu-id="161db-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="161db-172">Javascript</span><span class="sxs-lookup"><span data-stu-id="161db-172">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="161db-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="161db-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="161db-174">Java</span><span class="sxs-lookup"><span data-stu-id="161db-174">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getonedriveactivityusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="161db-175">响应</span><span class="sxs-lookup"><span data-stu-id="161db-175">Response</span></span>

<span data-ttu-id="161db-176">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="161db-176">The following is an example of the response.</span></span>

> <span data-ttu-id="161db-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="161db-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.siteActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 275

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.siteActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "viewedOrEdited": 93, 
      "synced": 26, 
      "sharedInternally": 6, 
      "sharedExternally": 0, 
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
