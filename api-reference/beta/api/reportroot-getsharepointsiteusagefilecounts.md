---
title: 'reportRoot: getSharePointSiteUsageFileCounts'
description: 获取跨所有网站的文件总数和活跃文件数。 如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c92f842326e2ea420ff4b2b0397e320c4bd0230a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869036"
---
# <a name="reportroot-getsharepointsiteusagefilecounts"></a><span data-ttu-id="d910b-104">reportRoot: getSharePointSiteUsageFileCounts</span><span class="sxs-lookup"><span data-stu-id="d910b-104">reportRoot: getSharePointSiteUsageFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d910b-105">获取跨所有网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="d910b-105">Get the total number of files across all sites and the number of active files.</span></span> <span data-ttu-id="d910b-106">如果文件（用户或系统）在指定时间段内被保存、同步、修改或共享，则视为活跃文件（用户或系统）。</span><span class="sxs-lookup"><span data-stu-id="d910b-106">A file (user or system) is considered active if it has been saved, synced, modified, or shared within the specified time period.</span></span>

> <span data-ttu-id="d910b-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - SharePoint 网站使用情况](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213)。</span><span class="sxs-lookup"><span data-stu-id="d910b-107">**Note:** For details about different report views and names, see [Office 365 Reports - SharePoint site usage](https://support.office.com/client/SharePoint-site-usage-4ecfb843-e5d5-464d-8bf6-7ed512a9b213).</span></span>

## <a name="permissions"></a><span data-ttu-id="d910b-108">权限</span><span class="sxs-lookup"><span data-stu-id="d910b-108">Permissions</span></span>

<span data-ttu-id="d910b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d910b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d910b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d910b-111">Permission type</span></span>                        | <span data-ttu-id="d910b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d910b-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d910b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d910b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="d910b-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d910b-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d910b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d910b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d910b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d910b-116">Not supported.</span></span>                           |
| <span data-ttu-id="d910b-117">应用</span><span class="sxs-lookup"><span data-stu-id="d910b-117">Application</span></span>                            | <span data-ttu-id="d910b-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d910b-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="d910b-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d910b-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d910b-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="d910b-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d910b-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d910b-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSharePointSiteUsageFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d910b-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="d910b-122">Function parameters</span></span>

<span data-ttu-id="d910b-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d910b-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d910b-124">参数</span><span class="sxs-lookup"><span data-stu-id="d910b-124">Parameter</span></span> | <span data-ttu-id="d910b-125">类型</span><span class="sxs-lookup"><span data-stu-id="d910b-125">Type</span></span>   | <span data-ttu-id="d910b-126">说明</span><span class="sxs-lookup"><span data-stu-id="d910b-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d910b-127">period</span><span class="sxs-lookup"><span data-stu-id="d910b-127">period</span></span>    | <span data-ttu-id="d910b-128">string</span><span class="sxs-lookup"><span data-stu-id="d910b-128">string</span></span> | <span data-ttu-id="d910b-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d910b-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d910b-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d910b-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d910b-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d910b-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d910b-132">必需。</span><span class="sxs-lookup"><span data-stu-id="d910b-132">Required.</span></span> |

<span data-ttu-id="d910b-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d910b-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d910b-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d910b-134">The default output type is text/csv.</span></span> <span data-ttu-id="d910b-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d910b-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d910b-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="d910b-136">Request headers</span></span>

| <span data-ttu-id="d910b-137">名称</span><span class="sxs-lookup"><span data-stu-id="d910b-137">Name</span></span>          | <span data-ttu-id="d910b-138">说明</span><span class="sxs-lookup"><span data-stu-id="d910b-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d910b-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="d910b-139">Authorization</span></span> | <span data-ttu-id="d910b-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d910b-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d910b-142">响应</span><span class="sxs-lookup"><span data-stu-id="d910b-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d910b-143">CSV</span><span class="sxs-lookup"><span data-stu-id="d910b-143">CSV</span></span>

<span data-ttu-id="d910b-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d910b-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d910b-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d910b-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d910b-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d910b-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d910b-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d910b-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d910b-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d910b-148">Report Refresh Date</span></span>
- <span data-ttu-id="d910b-149">网站类型</span><span class="sxs-lookup"><span data-stu-id="d910b-149">Site Type</span></span>
- <span data-ttu-id="d910b-150">总计</span><span class="sxs-lookup"><span data-stu-id="d910b-150">Total</span></span>
- <span data-ttu-id="d910b-151">活跃</span><span class="sxs-lookup"><span data-stu-id="d910b-151">Active</span></span>
- <span data-ttu-id="d910b-152">报表日期</span><span class="sxs-lookup"><span data-stu-id="d910b-152">Report Date</span></span>
- <span data-ttu-id="d910b-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="d910b-153">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d910b-154">JSON</span><span class="sxs-lookup"><span data-stu-id="d910b-154">JSON</span></span>

<span data-ttu-id="d910b-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d910b-155">If successful, this method returns a `200 OK` response code and a **[sharePointSiteUsageFileCounts](../resources/sharepointsiteusagefilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d910b-156">示例</span><span class="sxs-lookup"><span data-stu-id="d910b-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d910b-157">CSV</span><span class="sxs-lookup"><span data-stu-id="d910b-157">CSV</span></span>

<span data-ttu-id="d910b-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d910b-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d910b-159">请求</span><span class="sxs-lookup"><span data-stu-id="d910b-159">Request</span></span>

<span data-ttu-id="d910b-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d910b-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d910b-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="d910b-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d910b-162">C#</span><span class="sxs-lookup"><span data-stu-id="d910b-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d910b-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d910b-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d910b-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d910b-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d910b-165">响应</span><span class="sxs-lookup"><span data-stu-id="d910b-165">Response</span></span>

<span data-ttu-id="d910b-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d910b-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d910b-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d910b-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d910b-168">JSON</span><span class="sxs-lookup"><span data-stu-id="d910b-168">JSON</span></span>

<span data-ttu-id="d910b-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d910b-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d910b-170">请求</span><span class="sxs-lookup"><span data-stu-id="d910b-170">Request</span></span>

<span data-ttu-id="d910b-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d910b-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d910b-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="d910b-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getsharepointsiteusagefilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSharePointSiteUsageFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d910b-173">C#</span><span class="sxs-lookup"><span data-stu-id="d910b-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getsharepointsiteusagefilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d910b-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d910b-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getsharepointsiteusagefilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d910b-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d910b-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getsharepointsiteusagefilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d910b-176">响应</span><span class="sxs-lookup"><span data-stu-id="d910b-176">Response</span></span>

<span data-ttu-id="d910b-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d910b-177">The following is an example of the response.</span></span>

> <span data-ttu-id="d910b-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d910b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.sharePointSiteUsageFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.sharePointSiteUsageFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "siteType": "All", 
      "total": 25687, 
      "active": 209, 
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
