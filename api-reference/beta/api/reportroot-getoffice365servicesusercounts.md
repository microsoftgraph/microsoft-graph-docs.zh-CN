---
title: 'reportRoot: getOffice365ServicesUserCounts'
description: 按活动类型和服务获取用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: f9f117cb11280d573076cf9a7278c96f4f4e6dbe
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869106"
---
# <a name="reportroot-getoffice365servicesusercounts"></a><span data-ttu-id="b5179-103">reportRoot: getOffice365ServicesUserCounts</span><span class="sxs-lookup"><span data-stu-id="b5179-103">reportRoot: getOffice365ServicesUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5179-104">按活动类型和服务获取用户数。</span><span class="sxs-lookup"><span data-stu-id="b5179-104">Get the count of users by activity type and service.</span></span>

> <span data-ttu-id="b5179-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="b5179-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="b5179-106">权限</span><span class="sxs-lookup"><span data-stu-id="b5179-106">Permissions</span></span>

<span data-ttu-id="b5179-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5179-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5179-109">Permission type</span></span>                        | <span data-ttu-id="b5179-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5179-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="b5179-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5179-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5179-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5179-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="b5179-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5179-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5179-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5179-114">Not supported.</span></span>                           |
| <span data-ttu-id="b5179-115">应用</span><span class="sxs-lookup"><span data-stu-id="b5179-115">Application</span></span>                            | <span data-ttu-id="b5179-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5179-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="b5179-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="b5179-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="b5179-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="b5179-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="b5179-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5179-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ServicesUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="b5179-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="b5179-120">Function parameters</span></span>

<span data-ttu-id="b5179-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="b5179-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="b5179-122">参数</span><span class="sxs-lookup"><span data-stu-id="b5179-122">Parameter</span></span> | <span data-ttu-id="b5179-123">类型</span><span class="sxs-lookup"><span data-stu-id="b5179-123">Type</span></span>   | <span data-ttu-id="b5179-124">说明</span><span class="sxs-lookup"><span data-stu-id="b5179-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="b5179-125">period</span><span class="sxs-lookup"><span data-stu-id="b5179-125">period</span></span>    | <span data-ttu-id="b5179-126">string</span><span class="sxs-lookup"><span data-stu-id="b5179-126">string</span></span> | <span data-ttu-id="b5179-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b5179-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="b5179-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="b5179-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="b5179-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="b5179-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="b5179-130">必需。</span><span class="sxs-lookup"><span data-stu-id="b5179-130">Required.</span></span> |

<span data-ttu-id="b5179-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5179-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="b5179-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="b5179-132">The default output type is text/csv.</span></span> <span data-ttu-id="b5179-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="b5179-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5179-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5179-134">Request headers</span></span>

| <span data-ttu-id="b5179-135">名称</span><span class="sxs-lookup"><span data-stu-id="b5179-135">Name</span></span>          | <span data-ttu-id="b5179-136">说明</span><span class="sxs-lookup"><span data-stu-id="b5179-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="b5179-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5179-137">Authorization</span></span> | <span data-ttu-id="b5179-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5179-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="b5179-140">响应</span><span class="sxs-lookup"><span data-stu-id="b5179-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="b5179-141">CSV</span><span class="sxs-lookup"><span data-stu-id="b5179-141">CSV</span></span>

<span data-ttu-id="b5179-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="b5179-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="b5179-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="b5179-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="b5179-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="b5179-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="b5179-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="b5179-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="b5179-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="b5179-146">Report Refresh Date</span></span>
- <span data-ttu-id="b5179-147">Exchange 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-147">Exchange Active</span></span>
- <span data-ttu-id="b5179-148">Exchange 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-148">Exchange Inactive</span></span>
- <span data-ttu-id="b5179-149">OneDrive 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-149">OneDrive Active</span></span>
- <span data-ttu-id="b5179-150">OneDrive 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-150">OneDrive Inactive</span></span>
- <span data-ttu-id="b5179-151">SharePoint 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-151">SharePoint Active</span></span>
- <span data-ttu-id="b5179-152">SharePoint 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-152">SharePoint Inactive</span></span>
- <span data-ttu-id="b5179-153">Skype for Business 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-153">Skype For Business Active</span></span>
- <span data-ttu-id="b5179-154">Skype for Business 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-154">Skype For Business Inactive</span></span>
- <span data-ttu-id="b5179-155">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-155">Yammer Active</span></span>
- <span data-ttu-id="b5179-156">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-156">Yammer Inactive</span></span>
- <span data-ttu-id="b5179-157">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-157">Teams Active</span></span>
- <span data-ttu-id="b5179-158">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-158">Teams Inactive</span></span>
- <span data-ttu-id="b5179-159">Office 365 Active</span><span class="sxs-lookup"><span data-stu-id="b5179-159">Office 365 Active</span></span>
- <span data-ttu-id="b5179-160">Office 365 非活动</span><span class="sxs-lookup"><span data-stu-id="b5179-160">Office 365 Inactive</span></span>
- <span data-ttu-id="b5179-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="b5179-161">Report Period</span></span>

<span data-ttu-id="b5179-162">由世纪互联运营的 Microsoft Graph 中国不支持以下各列：</span><span class="sxs-lookup"><span data-stu-id="b5179-162">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b5179-163">Yammer 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-163">Yammer Active</span></span>
- <span data-ttu-id="b5179-164">Yammer 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-164">Yammer Inactive</span></span>
- <span data-ttu-id="b5179-165">Teams 活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-165">Teams Active</span></span>
- <span data-ttu-id="b5179-166">Teams 非活跃</span><span class="sxs-lookup"><span data-stu-id="b5179-166">Teams Inactive</span></span>

### <a name="json"></a><span data-ttu-id="b5179-167">JSON</span><span class="sxs-lookup"><span data-stu-id="b5179-167">JSON</span></span>

<span data-ttu-id="b5179-168">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="b5179-168">If successful, this method returns a `200 OK` response code and an **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="b5179-169">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="b5179-169">The following properties in **[office365ServicesUserCounts](../resources/office365servicesusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="b5179-170">yammerActive</span><span class="sxs-lookup"><span data-stu-id="b5179-170">yammerActive</span></span>
- <span data-ttu-id="b5179-171">yammerInactive</span><span class="sxs-lookup"><span data-stu-id="b5179-171">yammerInactive</span></span>
- <span data-ttu-id="b5179-172">teamsActive</span><span class="sxs-lookup"><span data-stu-id="b5179-172">teamsActive</span></span>
- <span data-ttu-id="b5179-173">teamsInactive</span><span class="sxs-lookup"><span data-stu-id="b5179-173">teamsInactive</span></span>

## <a name="example"></a><span data-ttu-id="b5179-174">示例</span><span class="sxs-lookup"><span data-stu-id="b5179-174">Example</span></span>

### <a name="csv"></a><span data-ttu-id="b5179-175">CSV</span><span class="sxs-lookup"><span data-stu-id="b5179-175">CSV</span></span>

<span data-ttu-id="b5179-176">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="b5179-176">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="b5179-177">请求</span><span class="sxs-lookup"><span data-stu-id="b5179-177">Request</span></span>

<span data-ttu-id="b5179-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5179-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5179-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5179-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5179-180">C#</span><span class="sxs-lookup"><span data-stu-id="b5179-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5179-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5179-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5179-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5179-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5179-183">响应</span><span class="sxs-lookup"><span data-stu-id="b5179-183">Response</span></span>

<span data-ttu-id="b5179-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5179-184">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="b5179-185">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="b5179-185">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="b5179-186">JSON</span><span class="sxs-lookup"><span data-stu-id="b5179-186">JSON</span></span> 

<span data-ttu-id="b5179-187">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="b5179-187">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="b5179-188">请求</span><span class="sxs-lookup"><span data-stu-id="b5179-188">Request</span></span>

<span data-ttu-id="b5179-189">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b5179-189">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5179-190">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5179-190">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365servicesusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ServicesUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5179-191">C#</span><span class="sxs-lookup"><span data-stu-id="b5179-191">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365servicesusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5179-192">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5179-192">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365servicesusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5179-193">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5179-193">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365servicesusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5179-194">响应</span><span class="sxs-lookup"><span data-stu-id="b5179-194">Response</span></span>

<span data-ttu-id="b5179-195">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="b5179-195">The following is an example of the response.</span></span>

> <span data-ttu-id="b5179-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b5179-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
