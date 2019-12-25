---
title: 'reportRoot: getOneDriveUsageAccountCounts'
description: 获取 OneDrive for Business 活跃网站数趋势。 用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 57555639e2b4702d1408b76e0ce7ae35fc3dcb31
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867478"
---
# <a name="reportroot-getonedriveusageaccountcounts"></a><span data-ttu-id="a980e-104">reportRoot: getOneDriveUsageAccountCounts</span><span class="sxs-lookup"><span data-stu-id="a980e-104">reportRoot: getOneDriveUsageAccountCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a980e-105">获取 OneDrive for Business 活跃网站数趋势。</span><span class="sxs-lookup"><span data-stu-id="a980e-105">Get the trend in the number of active OneDrive for Business sites.</span></span> <span data-ttu-id="a980e-106">用户在其中查看、修改、上传、下载、共享或同步文件的任何网站都被视为活跃网站。</span><span class="sxs-lookup"><span data-stu-id="a980e-106">Any site on which users viewed, modified, uploaded, downloaded, shared, or synced files is considered an active site.</span></span>

> <span data-ttu-id="a980e-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - OneDrive for Business 使用情况](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680)。</span><span class="sxs-lookup"><span data-stu-id="a980e-107">**Note:** For details about different report views and names, see [Office 365 Reports - OneDrive for Business usage](https://support.office.com/client/OneDrive-for-Business-usage-0de3b312-c4e8-4e4b-a02d-32b2f726a680).</span></span>

## <a name="permissions"></a><span data-ttu-id="a980e-108">权限</span><span class="sxs-lookup"><span data-stu-id="a980e-108">Permissions</span></span>

<span data-ttu-id="a980e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a980e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a980e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a980e-111">Permission type</span></span>                        | <span data-ttu-id="a980e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a980e-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a980e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a980e-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a980e-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a980e-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a980e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a980e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a980e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a980e-116">Not supported.</span></span>                           |
| <span data-ttu-id="a980e-117">应用</span><span class="sxs-lookup"><span data-stu-id="a980e-117">Application</span></span>                            | <span data-ttu-id="a980e-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a980e-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="a980e-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a980e-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a980e-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a980e-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a980e-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a980e-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOneDriveUsageAccountCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a980e-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="a980e-122">Function parameters</span></span>

<span data-ttu-id="a980e-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a980e-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a980e-124">参数</span><span class="sxs-lookup"><span data-stu-id="a980e-124">Parameter</span></span> | <span data-ttu-id="a980e-125">类型</span><span class="sxs-lookup"><span data-stu-id="a980e-125">Type</span></span>   | <span data-ttu-id="a980e-126">说明</span><span class="sxs-lookup"><span data-stu-id="a980e-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a980e-127">period</span><span class="sxs-lookup"><span data-stu-id="a980e-127">period</span></span>    | <span data-ttu-id="a980e-128">string</span><span class="sxs-lookup"><span data-stu-id="a980e-128">string</span></span> | <span data-ttu-id="a980e-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a980e-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a980e-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a980e-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a980e-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a980e-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a980e-132">必需。</span><span class="sxs-lookup"><span data-stu-id="a980e-132">Required.</span></span> |

<span data-ttu-id="a980e-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a980e-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a980e-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a980e-134">The default output type is text/csv.</span></span> <span data-ttu-id="a980e-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a980e-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a980e-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a980e-136">Request headers</span></span>

| <span data-ttu-id="a980e-137">名称</span><span class="sxs-lookup"><span data-stu-id="a980e-137">Name</span></span>          | <span data-ttu-id="a980e-138">说明</span><span class="sxs-lookup"><span data-stu-id="a980e-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a980e-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a980e-139">Authorization</span></span> | <span data-ttu-id="a980e-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a980e-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a980e-142">响应</span><span class="sxs-lookup"><span data-stu-id="a980e-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a980e-143">CSV</span><span class="sxs-lookup"><span data-stu-id="a980e-143">CSV</span></span>

<span data-ttu-id="a980e-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a980e-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a980e-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a980e-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a980e-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a980e-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a980e-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a980e-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a980e-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a980e-148">Report Refresh Date</span></span>
- <span data-ttu-id="a980e-149">网站类型</span><span class="sxs-lookup"><span data-stu-id="a980e-149">Site Type</span></span>
- <span data-ttu-id="a980e-150">总计</span><span class="sxs-lookup"><span data-stu-id="a980e-150">Total</span></span>
- <span data-ttu-id="a980e-151">活跃</span><span class="sxs-lookup"><span data-stu-id="a980e-151">Active</span></span>
- <span data-ttu-id="a980e-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="a980e-152">Report Date</span></span>
- <span data-ttu-id="a980e-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="a980e-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a980e-154">JSON</span><span class="sxs-lookup"><span data-stu-id="a980e-154">JSON</span></span>

<span data-ttu-id="a980e-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a980e-155">If successful, this method returns a `200 OK` response code and a **[oneDriveUsageAccountCounts](../resources/onedriveusageaccountcounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a980e-156">示例</span><span class="sxs-lookup"><span data-stu-id="a980e-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a980e-157">CSV</span><span class="sxs-lookup"><span data-stu-id="a980e-157">CSV</span></span>

<span data-ttu-id="a980e-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a980e-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a980e-159">请求</span><span class="sxs-lookup"><span data-stu-id="a980e-159">Request</span></span>

<span data-ttu-id="a980e-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a980e-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a980e-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="a980e-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a980e-162">C#</span><span class="sxs-lookup"><span data-stu-id="a980e-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a980e-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a980e-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a980e-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a980e-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a980e-165">响应</span><span class="sxs-lookup"><span data-stu-id="a980e-165">Response</span></span>

<span data-ttu-id="a980e-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a980e-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a980e-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a980e-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a980e-168">JSON</span><span class="sxs-lookup"><span data-stu-id="a980e-168">JSON</span></span>

<span data-ttu-id="a980e-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a980e-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a980e-170">请求</span><span class="sxs-lookup"><span data-stu-id="a980e-170">Request</span></span>

<span data-ttu-id="a980e-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a980e-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a980e-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a980e-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getonedriveusageaccountcounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOneDriveUsageAccountCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a980e-173">C#</span><span class="sxs-lookup"><span data-stu-id="a980e-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getonedriveusageaccountcounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a980e-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a980e-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getonedriveusageaccountcounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a980e-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a980e-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getonedriveusageaccountcounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a980e-176">响应</span><span class="sxs-lookup"><span data-stu-id="a980e-176">Response</span></span>

<span data-ttu-id="a980e-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a980e-177">The following is an example of the response.</span></span>

> <span data-ttu-id="a980e-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a980e-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.oneDriveUsageAccountCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.oneDriveUsageAccountCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 207, 
      "active": 89, 
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
