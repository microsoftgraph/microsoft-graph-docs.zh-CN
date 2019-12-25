---
title: 'reportRoot: getOneDriveUsageAccountDetail'
description: 获取帐户的 OneDrive 使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 241d0557d5bafab69f3e5f8500da1d3acb22a9aa
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869078"
---
# <a name="reportroot-getonedriveusageaccountdetail"></a><span data-ttu-id="d72e7-103">reportRoot: getOneDriveUsageAccountDetail</span><span class="sxs-lookup"><span data-stu-id="d72e7-103">reportRoot: getOneDriveUsageAccountDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d72e7-104">获取帐户的 OneDrive 使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d72e7-104">Get details about OneDrive usage by account.</span></span>

> <span data-ttu-id="d72e7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="d72e7-105">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="d72e7-106">权限</span><span class="sxs-lookup"><span data-stu-id="d72e7-106">Permissions</span></span>

<span data-ttu-id="d72e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d72e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d72e7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d72e7-109">Permission type</span></span>                        | <span data-ttu-id="d72e7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d72e7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d72e7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d72e7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d72e7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d72e7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d72e7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d72e7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d72e7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d72e7-114">Not supported.</span></span>                           |
| <span data-ttu-id="d72e7-115">应用</span><span class="sxs-lookup"><span data-stu-id="d72e7-115">Application</span></span>                            | <span data-ttu-id="d72e7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d72e7-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="d72e7-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d72e7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d72e7-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="d72e7-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d72e7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d72e7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountDetail(period='{period_value}')
GET /reports/getOneDriveUsageAccountDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="d72e7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d72e7-120">Function parameters</span></span>

<span data-ttu-id="d72e7-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d72e7-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="d72e7-122">参数</span><span class="sxs-lookup"><span data-stu-id="d72e7-122">Parameter</span></span> | <span data-ttu-id="d72e7-123">类型</span><span class="sxs-lookup"><span data-stu-id="d72e7-123">Type</span></span>   | <span data-ttu-id="d72e7-124">说明</span><span class="sxs-lookup"><span data-stu-id="d72e7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d72e7-125">period</span><span class="sxs-lookup"><span data-stu-id="d72e7-125">period</span></span>    | <span data-ttu-id="d72e7-126">string</span><span class="sxs-lookup"><span data-stu-id="d72e7-126">string</span></span> | <span data-ttu-id="d72e7-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d72e7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d72e7-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d72e7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d72e7-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d72e7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="d72e7-130">date</span><span class="sxs-lookup"><span data-stu-id="d72e7-130">date</span></span>      | <span data-ttu-id="d72e7-131">Date</span><span class="sxs-lookup"><span data-stu-id="d72e7-131">Date</span></span>   | <span data-ttu-id="d72e7-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="d72e7-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="d72e7-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="d72e7-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="d72e7-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="d72e7-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="d72e7-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="d72e7-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="d72e7-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d72e7-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d72e7-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d72e7-137">The default output type is text/csv.</span></span> <span data-ttu-id="d72e7-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d72e7-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d72e7-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="d72e7-139">Request headers</span></span>

| <span data-ttu-id="d72e7-140">名称</span><span class="sxs-lookup"><span data-stu-id="d72e7-140">Name</span></span>          | <span data-ttu-id="d72e7-141">说明</span><span class="sxs-lookup"><span data-stu-id="d72e7-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d72e7-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="d72e7-142">Authorization</span></span> | <span data-ttu-id="d72e7-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d72e7-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d72e7-145">响应</span><span class="sxs-lookup"><span data-stu-id="d72e7-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d72e7-146">CSV</span><span class="sxs-lookup"><span data-stu-id="d72e7-146">CSV</span></span>

<span data-ttu-id="d72e7-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d72e7-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d72e7-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d72e7-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d72e7-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d72e7-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d72e7-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d72e7-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d72e7-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d72e7-151">Report Refresh Date</span></span>
- <span data-ttu-id="d72e7-152">网站 URL</span><span class="sxs-lookup"><span data-stu-id="d72e7-152">Site URL</span></span>
- <span data-ttu-id="d72e7-153">所有者显示名称</span><span class="sxs-lookup"><span data-stu-id="d72e7-153">Owner Display Name</span></span>
- <span data-ttu-id="d72e7-154">已删除</span><span class="sxs-lookup"><span data-stu-id="d72e7-154">Is Deleted</span></span>
- <span data-ttu-id="d72e7-155">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="d72e7-155">Last Activity Date</span></span>
- <span data-ttu-id="d72e7-156">文件数</span><span class="sxs-lookup"><span data-stu-id="d72e7-156">File Count</span></span>
- <span data-ttu-id="d72e7-157">活跃文件数</span><span class="sxs-lookup"><span data-stu-id="d72e7-157">Active File Count</span></span>
- <span data-ttu-id="d72e7-158">已使用的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="d72e7-158">Storage Used (Byte)</span></span>
- <span data-ttu-id="d72e7-159">已分配的存储（字节）</span><span class="sxs-lookup"><span data-stu-id="d72e7-159">Storage Allocated (Byte)</span></span>
- <span data-ttu-id="d72e7-160">所有者主体名称</span><span class="sxs-lookup"><span data-stu-id="d72e7-160">Owner Principal Name</span></span>
- <span data-ttu-id="d72e7-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="d72e7-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d72e7-162">JSON</span><span class="sxs-lookup"><span data-stu-id="d72e7-162">JSON</span></span>

<span data-ttu-id="d72e7-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d72e7-163">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountDetail](../resources/onedriveusageaccountdetail.md)** object in the response body.</span></span>

<span data-ttu-id="d72e7-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="d72e7-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="d72e7-165">示例</span><span class="sxs-lookup"><span data-stu-id="d72e7-165">Example</span></span>

<span data-ttu-id="d72e7-166">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d72e7-166">The following is an example that outputs CSV.</span></span>

### <a name="csv"></a><span data-ttu-id="d72e7-167">CSV</span><span class="sxs-lookup"><span data-stu-id="d72e7-167">CSV</span></span>

#### <a name="request"></a><span data-ttu-id="d72e7-168">请求</span><span class="sxs-lookup"><span data-stu-id="d72e7-168">Request</span></span>

<span data-ttu-id="d72e7-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d72e7-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d72e7-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72e7-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d72e7-171">C#</span><span class="sxs-lookup"><span data-stu-id="d72e7-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d72e7-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72e7-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d72e7-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72e7-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d72e7-174">响应</span><span class="sxs-lookup"><span data-stu-id="d72e7-174">Response</span></span>

<span data-ttu-id="d72e7-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d72e7-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d72e7-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d72e7-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d72e7-177">JSON</span><span class="sxs-lookup"><span data-stu-id="d72e7-177">JSON</span></span>

<span data-ttu-id="d72e7-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d72e7-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d72e7-179">请求</span><span class="sxs-lookup"><span data-stu-id="d72e7-179">Request</span></span>

<span data-ttu-id="d72e7-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d72e7-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d72e7-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="d72e7-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d72e7-182">C#</span><span class="sxs-lookup"><span data-stu-id="d72e7-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d72e7-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d72e7-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d72e7-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d72e7-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d72e7-185">响应</span><span class="sxs-lookup"><span data-stu-id="d72e7-185">Response</span></span>

<span data-ttu-id="d72e7-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d72e7-186">The following is an example of the response.</span></span>

> <span data-ttu-id="d72e7-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d72e7-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
