---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b1dda8b0f071ea3d5ea7aaaed051b597cd503fe1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723005"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="24591-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="24591-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="24591-104">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="24591-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="24591-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="24591-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="24591-106">权限</span><span class="sxs-lookup"><span data-stu-id="24591-106">Permissions</span></span>

<span data-ttu-id="24591-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="24591-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24591-109">Permission type</span></span>                        | <span data-ttu-id="24591-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24591-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="24591-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24591-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24591-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24591-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="24591-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24591-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24591-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24591-114">Not supported.</span></span>                           |
| <span data-ttu-id="24591-115">应用</span><span class="sxs-lookup"><span data-stu-id="24591-115">Application</span></span>                            | <span data-ttu-id="24591-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="24591-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="24591-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24591-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="24591-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="24591-118">Function parameters</span></span>

<span data-ttu-id="24591-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="24591-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="24591-120">参数</span><span class="sxs-lookup"><span data-stu-id="24591-120">Parameter</span></span> | <span data-ttu-id="24591-121">类型</span><span class="sxs-lookup"><span data-stu-id="24591-121">Type</span></span>   | <span data-ttu-id="24591-122">说明</span><span class="sxs-lookup"><span data-stu-id="24591-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="24591-123">period</span><span class="sxs-lookup"><span data-stu-id="24591-123">period</span></span>    | <span data-ttu-id="24591-124">string</span><span class="sxs-lookup"><span data-stu-id="24591-124">string</span></span> | <span data-ttu-id="24591-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="24591-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="24591-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="24591-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="24591-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="24591-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="24591-128">必需。</span><span class="sxs-lookup"><span data-stu-id="24591-128">Required.</span></span> |

<span data-ttu-id="24591-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="24591-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="24591-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="24591-130">The default output type is text/csv.</span></span> <span data-ttu-id="24591-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="24591-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24591-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="24591-132">Request headers</span></span>

| <span data-ttu-id="24591-133">名称</span><span class="sxs-lookup"><span data-stu-id="24591-133">Name</span></span>          | <span data-ttu-id="24591-134">说明</span><span class="sxs-lookup"><span data-stu-id="24591-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="24591-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="24591-135">Authorization</span></span> | <span data-ttu-id="24591-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24591-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="24591-138">响应</span><span class="sxs-lookup"><span data-stu-id="24591-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="24591-139">CSV</span><span class="sxs-lookup"><span data-stu-id="24591-139">CSV</span></span>

<span data-ttu-id="24591-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="24591-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="24591-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="24591-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="24591-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="24591-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="24591-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="24591-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="24591-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="24591-144">Report Refresh Date</span></span>
- <span data-ttu-id="24591-145">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-145">Exchange Active</span></span>
- <span data-ttu-id="24591-146">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-146">Exchange Inactive</span></span>
- <span data-ttu-id="24591-147">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-147">OneDrive Active</span></span>
- <span data-ttu-id="24591-148">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-148">OneDrive Inactive</span></span>
- <span data-ttu-id="24591-149">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-149">SharePoint Active</span></span>
- <span data-ttu-id="24591-150">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-150">SharePoint Inactive</span></span>
- <span data-ttu-id="24591-151">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-151">Skype For Business Active</span></span>
- <span data-ttu-id="24591-152">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-152">Skype For Business Inactive</span></span>
- <span data-ttu-id="24591-153">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-153">Yammer Active</span></span>
- <span data-ttu-id="24591-154">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-154">Yammer Inactive</span></span>
- <span data-ttu-id="24591-155">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-155">Teams Active</span></span>
- <span data-ttu-id="24591-156">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-156">Teams Inactive</span></span>
- <span data-ttu-id="24591-157">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="24591-157">Office 365 Active</span></span>
- <span data-ttu-id="24591-158">Office 365 非活动</span><span class="sxs-lookup"><span data-stu-id="24591-158">Office 365 Inactive</span></span>
- <span data-ttu-id="24591-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="24591-159">Report Period</span></span>

<span data-ttu-id="24591-160">由世纪互联运营的 Microsoft Graph 中国不支持以下各列:</span><span class="sxs-lookup"><span data-stu-id="24591-160">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="24591-161">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-161">Yammer Active</span></span>
- <span data-ttu-id="24591-162">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-162">Yammer Inactive</span></span>
- <span data-ttu-id="24591-163">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="24591-163">Teams Active</span></span>
- <span data-ttu-id="24591-164">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="24591-164">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="24591-165">JSON</span><span class="sxs-lookup"><span data-stu-id="24591-165">JSON</span></span>

<span data-ttu-id="24591-166">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="24591-166">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="24591-167">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象中的以下属性:</span><span class="sxs-lookup"><span data-stu-id="24591-167">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="24591-168">yammerActive</span><span class="sxs-lookup"><span data-stu-id="24591-168">yammerActive</span></span>
- <span data-ttu-id="24591-169">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="24591-169">yammerInactive</span></span>
- <span data-ttu-id="24591-170">teamsActive</span><span class="sxs-lookup"><span data-stu-id="24591-170">teamsActive</span></span>
- <span data-ttu-id="24591-171">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="24591-171">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="24591-172">示例</span><span class="sxs-lookup"><span data-stu-id="24591-172">Example</span></span>

### <a name="csv"></a><span data-ttu-id="24591-173">CSV</span><span class="sxs-lookup"><span data-stu-id="24591-173">CSV</span></span>

<span data-ttu-id="24591-174">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="24591-174">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="24591-175">请求</span><span class="sxs-lookup"><span data-stu-id="24591-175">Request</span></span>

<span data-ttu-id="24591-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="24591-176">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="24591-177">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="24591-177">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24591-178">C#</span><span class="sxs-lookup"><span data-stu-id="24591-178">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24591-179">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24591-179">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24591-180">目标-C</span><span class="sxs-lookup"><span data-stu-id="24591-180">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24591-181">响应</span><span class="sxs-lookup"><span data-stu-id="24591-181">Response</span></span>

<span data-ttu-id="24591-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="24591-182">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="24591-183">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="24591-183">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Exchange Active,Exchange Inactive,OneDrive Active,OneDrive Inactive,SharePoint Active,SharePoint Inactive,Skype For Business Active,Skype For Business Inactive,Yammer Active,Yammer Inactive,Teams Active,Teams Inactive,Office 365 Active,Office 365 Inactive,Report Period
```

### <a name="json"></a><span data-ttu-id="24591-184">JSON</span><span class="sxs-lookup"><span data-stu-id="24591-184">JSON</span></span> 

<span data-ttu-id="24591-185">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="24591-185">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="24591-186">请求</span><span class="sxs-lookup"><span data-stu-id="24591-186">Request</span></span>

<span data-ttu-id="24591-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="24591-187">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="24591-188">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="24591-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="24591-189">C#</span><span class="sxs-lookup"><span data-stu-id="24591-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="24591-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="24591-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="24591-191">目标-C</span><span class="sxs-lookup"><span data-stu-id="24591-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="24591-192">响应</span><span class="sxs-lookup"><span data-stu-id="24591-192">Response</span></span>

<span data-ttu-id="24591-193">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="24591-193">The following is an example of the response.</span></span>

> <span data-ttu-id="24591-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="24591-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ServicesUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 458

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ServicesUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "exchangeActive": 2591, 
      "exchangeInactive": 1426, 
      "oneDriveActive": 1800, 
      "oneDriveInactive": 2451, 
      "sharePointActive": 2286, 
      "sharePointInactive": 1815, 
      "skypeForBusinessActive": 2463, 
      "skypeForBusinessInactive": 1947, 
      "yammerActive": 473, 
      "yammerInactive": 2526, 
      "teamsActive": 846, 
      "teamsInactive": 1960, 
      "office365Active": 2791,
      "office365Inactive": 503,
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
