---
title: 'reportRoot: getOffice365GroupsActivityFileCounts'
description: 获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 8262cc6759a3de4e85fae2fb5d4817248ea03efc
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867526"
---
# <a name="reportroot-getoffice365groupsactivityfilecounts"></a><span data-ttu-id="d7cc7-103">reportRoot: getOffice365GroupsActivityFileCounts</span><span class="sxs-lookup"><span data-stu-id="d7cc7-103">reportRoot: getOffice365GroupsActivityFileCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7cc7-104">获取跨与 Office 365 组相关联的所有组网站的文件总数和活跃文件数。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-104">Get the total number of files and how many of them were active across all group sites associated with an Office 365 Group.</span></span>

> <span data-ttu-id="d7cc7-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Office 365 组](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40)。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-105">**Note:** For details about different report views and names, see [Office 365 Reports - Office 365 groups](https://support.office.com/client/Office-365-groups-a27f1a99-3557-4f85-9560-a28e3d822a40).</span></span>

## <a name="permissions"></a><span data-ttu-id="d7cc7-106">权限</span><span class="sxs-lookup"><span data-stu-id="d7cc7-106">Permissions</span></span>

<span data-ttu-id="d7cc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d7cc7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7cc7-109">Permission type</span></span>                        | <span data-ttu-id="d7cc7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7cc7-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="d7cc7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7cc7-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d7cc7-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7cc7-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="d7cc7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7cc7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7cc7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-114">Not supported.</span></span>                           |
| <span data-ttu-id="d7cc7-115">应用</span><span class="sxs-lookup"><span data-stu-id="d7cc7-115">Application</span></span>                            | <span data-ttu-id="d7cc7-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="d7cc7-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="d7cc7-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="d7cc7-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="d7cc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7cc7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365GroupsActivityFileCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="d7cc7-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="d7cc7-120">Function parameters</span></span>

<span data-ttu-id="d7cc7-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="d7cc7-122">参数</span><span class="sxs-lookup"><span data-stu-id="d7cc7-122">Parameter</span></span> | <span data-ttu-id="d7cc7-123">类型</span><span class="sxs-lookup"><span data-stu-id="d7cc7-123">Type</span></span>   | <span data-ttu-id="d7cc7-124">说明</span><span class="sxs-lookup"><span data-stu-id="d7cc7-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="d7cc7-125">period</span><span class="sxs-lookup"><span data-stu-id="d7cc7-125">period</span></span>    | <span data-ttu-id="d7cc7-126">string</span><span class="sxs-lookup"><span data-stu-id="d7cc7-126">string</span></span> | <span data-ttu-id="d7cc7-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="d7cc7-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="d7cc7-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="d7cc7-130">必需。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-130">Required.</span></span> |

<span data-ttu-id="d7cc7-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="d7cc7-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-132">The default output type is text/csv.</span></span> <span data-ttu-id="d7cc7-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d7cc7-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7cc7-134">Request headers</span></span>

| <span data-ttu-id="d7cc7-135">名称</span><span class="sxs-lookup"><span data-stu-id="d7cc7-135">Name</span></span>          | <span data-ttu-id="d7cc7-136">说明</span><span class="sxs-lookup"><span data-stu-id="d7cc7-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="d7cc7-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7cc7-137">Authorization</span></span> | <span data-ttu-id="d7cc7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="d7cc7-140">响应</span><span class="sxs-lookup"><span data-stu-id="d7cc7-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="d7cc7-141">CSV</span><span class="sxs-lookup"><span data-stu-id="d7cc7-141">CSV</span></span>

<span data-ttu-id="d7cc7-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="d7cc7-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="d7cc7-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="d7cc7-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="d7cc7-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="d7cc7-146">Report Refresh Date</span></span>
- <span data-ttu-id="d7cc7-147">总计</span><span class="sxs-lookup"><span data-stu-id="d7cc7-147">Total</span></span>
- <span data-ttu-id="d7cc7-148">活跃</span><span class="sxs-lookup"><span data-stu-id="d7cc7-148">Active</span></span>
- <span data-ttu-id="d7cc7-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="d7cc7-149">Report Date</span></span>
- <span data-ttu-id="d7cc7-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="d7cc7-150">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="d7cc7-151">JSON</span><span class="sxs-lookup"><span data-stu-id="d7cc7-151">JSON</span></span>

<span data-ttu-id="d7cc7-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-152">If successful, this method returns a `200 OK` response code and an **[office365GroupsActivityFileCounts](../resources/office365groupsactivityfilecounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d7cc7-153">示例</span><span class="sxs-lookup"><span data-stu-id="d7cc7-153">Example</span></span>

### <a name="csv"></a><span data-ttu-id="d7cc7-154">CSV</span><span class="sxs-lookup"><span data-stu-id="d7cc7-154">CSV</span></span>

<span data-ttu-id="d7cc7-155">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-155">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="d7cc7-156">请求</span><span class="sxs-lookup"><span data-stu-id="d7cc7-156">Request</span></span>

<span data-ttu-id="d7cc7-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-157">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d7cc7-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7cc7-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7cc7-159">C#</span><span class="sxs-lookup"><span data-stu-id="d7cc7-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityfilecounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7cc7-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7cc7-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityfilecounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7cc7-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7cc7-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityfilecounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7cc7-162">响应</span><span class="sxs-lookup"><span data-stu-id="d7cc7-162">Response</span></span>

<span data-ttu-id="d7cc7-163">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-163">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="d7cc7-164">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-164">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="d7cc7-165">JSON</span><span class="sxs-lookup"><span data-stu-id="d7cc7-165">JSON</span></span>

<span data-ttu-id="d7cc7-166">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-166">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="d7cc7-167">请求</span><span class="sxs-lookup"><span data-stu-id="d7cc7-167">Request</span></span>

<span data-ttu-id="d7cc7-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d7cc7-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7cc7-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365groupsactivityfilecounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365GroupsActivityFileCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d7cc7-170">C#</span><span class="sxs-lookup"><span data-stu-id="d7cc7-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365groupsactivityfilecounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7cc7-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7cc7-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365groupsactivityfilecounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d7cc7-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7cc7-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365groupsactivityfilecounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="d7cc7-173">响应</span><span class="sxs-lookup"><span data-stu-id="d7cc7-173">Response</span></span>

<span data-ttu-id="d7cc7-174">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-174">The following is an example of the response.</span></span>

> <span data-ttu-id="d7cc7-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="d7cc7-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365GroupsActivityFileCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 229

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365GroupsActivityFileCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "total": 26, 
      "active": 5, 
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
