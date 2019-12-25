---
title: 'reportRoot: getOffice365ActiveUserCounts'
description: 按产品获取报表周期内的每日活跃用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: d92293e3daba5ba86d18ecdea347d70782e13170
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867552"
---
# <a name="reportroot-getoffice365activeusercounts"></a><span data-ttu-id="0b292-103">reportRoot: getOffice365ActiveUserCounts</span><span class="sxs-lookup"><span data-stu-id="0b292-103">reportRoot: getOffice365ActiveUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0b292-104">按产品获取报表周期内的每日活跃用户数。</span><span class="sxs-lookup"><span data-stu-id="0b292-104">Get the count of daily active users in the reporting period by product.</span></span>

> <span data-ttu-id="0b292-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 活跃用户](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d)。</span><span class="sxs-lookup"><span data-stu-id="0b292-105">**Note:** For details about different report views and names, see [Office 365 Reports - Active Users](https://support.office.com/client/Active-Users-fc1cf1d0-cd84-43fd-adb7-a4c4dfa8112d).</span></span>

## <a name="permissions"></a><span data-ttu-id="0b292-106">权限</span><span class="sxs-lookup"><span data-stu-id="0b292-106">Permissions</span></span>

<span data-ttu-id="0b292-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0b292-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b292-109">Permission type</span></span>                        | <span data-ttu-id="0b292-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b292-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="0b292-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b292-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="0b292-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b292-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="0b292-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b292-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0b292-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b292-114">Not supported.</span></span>                           |
| <span data-ttu-id="0b292-115">应用</span><span class="sxs-lookup"><span data-stu-id="0b292-115">Application</span></span>                            | <span data-ttu-id="0b292-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="0b292-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="0b292-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="0b292-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="0b292-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="0b292-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="0b292-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b292-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getOffice365ActiveUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="0b292-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="0b292-120">Function parameters</span></span>

<span data-ttu-id="0b292-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="0b292-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="0b292-122">参数</span><span class="sxs-lookup"><span data-stu-id="0b292-122">Parameter</span></span> | <span data-ttu-id="0b292-123">类型</span><span class="sxs-lookup"><span data-stu-id="0b292-123">Type</span></span>   | <span data-ttu-id="0b292-124">说明</span><span class="sxs-lookup"><span data-stu-id="0b292-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="0b292-125">period</span><span class="sxs-lookup"><span data-stu-id="0b292-125">period</span></span>    | <span data-ttu-id="0b292-126">string</span><span class="sxs-lookup"><span data-stu-id="0b292-126">string</span></span> | <span data-ttu-id="0b292-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b292-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="0b292-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="0b292-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="0b292-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="0b292-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="0b292-130">必需。</span><span class="sxs-lookup"><span data-stu-id="0b292-130">Required.</span></span> |

<span data-ttu-id="0b292-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0b292-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="0b292-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="0b292-132">The default output type is text/csv.</span></span> <span data-ttu-id="0b292-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="0b292-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b292-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b292-134">Request headers</span></span>

| <span data-ttu-id="0b292-135">名称</span><span class="sxs-lookup"><span data-stu-id="0b292-135">Name</span></span>          | <span data-ttu-id="0b292-136">说明</span><span class="sxs-lookup"><span data-stu-id="0b292-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="0b292-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b292-137">Authorization</span></span> | <span data-ttu-id="0b292-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b292-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="0b292-140">响应</span><span class="sxs-lookup"><span data-stu-id="0b292-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="0b292-141">CSV</span><span class="sxs-lookup"><span data-stu-id="0b292-141">CSV</span></span>

<span data-ttu-id="0b292-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="0b292-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="0b292-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="0b292-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="0b292-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="0b292-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="0b292-145">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="0b292-145">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="0b292-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="0b292-146">Report Refresh Date</span></span>
- <span data-ttu-id="0b292-147">Office 365</span><span class="sxs-lookup"><span data-stu-id="0b292-147">Office 365</span></span>
- <span data-ttu-id="0b292-148">Exchange</span><span class="sxs-lookup"><span data-stu-id="0b292-148">Exchange</span></span>
- <span data-ttu-id="0b292-149">OneDrive</span><span class="sxs-lookup"><span data-stu-id="0b292-149">OneDrive</span></span>
- <span data-ttu-id="0b292-150">SharePoint</span><span class="sxs-lookup"><span data-stu-id="0b292-150">SharePoint</span></span>
- <span data-ttu-id="0b292-151">Skype for Business</span><span class="sxs-lookup"><span data-stu-id="0b292-151">Skype For Business</span></span> 
- <span data-ttu-id="0b292-152">Yammer</span><span class="sxs-lookup"><span data-stu-id="0b292-152">Yammer</span></span>
- <span data-ttu-id="0b292-153">Teams</span><span class="sxs-lookup"><span data-stu-id="0b292-153">Teams</span></span>
- <span data-ttu-id="0b292-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="0b292-154">Report Date</span></span>
- <span data-ttu-id="0b292-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="0b292-155">Report Period</span></span>

<span data-ttu-id="0b292-156">由世纪互联运营的 Microsoft Graph 中国不支持以下各列：</span><span class="sxs-lookup"><span data-stu-id="0b292-156">The following columns are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="0b292-157">Yammer</span><span class="sxs-lookup"><span data-stu-id="0b292-157">Yammer</span></span>
- <span data-ttu-id="0b292-158">Teams</span><span class="sxs-lookup"><span data-stu-id="0b292-158">Teams</span></span>

### <a name="json"></a><span data-ttu-id="0b292-159">JSON</span><span class="sxs-lookup"><span data-stu-id="0b292-159">JSON</span></span>

<span data-ttu-id="0b292-160">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="0b292-160">If successful, this method returns a `200 OK` response code and an **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object in the response body.</span></span>

<span data-ttu-id="0b292-161">由世纪互联运营的 Microsoft Graph 中国不支持**[office365ActiveUserCounts](../resources/office365activeusercounts.md)** 对象中的以下属性：</span><span class="sxs-lookup"><span data-stu-id="0b292-161">The following properties in **[office365ActiveUserCounts](../resources/office365activeusercounts.md)** object are not supported in Microsoft Graph China operated by 21Vianet:</span></span>

- <span data-ttu-id="0b292-162">yammer</span><span class="sxs-lookup"><span data-stu-id="0b292-162">yammer</span></span>
- <span data-ttu-id="0b292-163">协作</span><span class="sxs-lookup"><span data-stu-id="0b292-163">teams</span></span>

## <a name="example"></a><span data-ttu-id="0b292-164">示例</span><span class="sxs-lookup"><span data-stu-id="0b292-164">Example</span></span>

### <a name="csv"></a><span data-ttu-id="0b292-165">CSV</span><span class="sxs-lookup"><span data-stu-id="0b292-165">CSV</span></span>

<span data-ttu-id="0b292-166">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="0b292-166">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="0b292-167">请求</span><span class="sxs-lookup"><span data-stu-id="0b292-167">Request</span></span>

<span data-ttu-id="0b292-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b292-168">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b292-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b292-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b292-170">C#</span><span class="sxs-lookup"><span data-stu-id="0b292-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b292-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b292-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b292-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b292-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b292-173">响应</span><span class="sxs-lookup"><span data-stu-id="0b292-173">Response</span></span>

<span data-ttu-id="0b292-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0b292-174">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="0b292-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="0b292-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Office 365,Exchange,OneDrive,SharePoint,Skype For Business,Yammer,Teams,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="0b292-176">JSON</span><span class="sxs-lookup"><span data-stu-id="0b292-176">JSON</span></span>

<span data-ttu-id="0b292-177">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="0b292-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="0b292-178">请求</span><span class="sxs-lookup"><span data-stu-id="0b292-178">Request</span></span>

<span data-ttu-id="0b292-179">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0b292-179">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="0b292-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b292-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getoffice365activeusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getOffice365ActiveUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0b292-181">C#</span><span class="sxs-lookup"><span data-stu-id="0b292-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getoffice365activeusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0b292-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b292-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getoffice365activeusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0b292-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b292-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getoffice365activeusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b292-184">响应</span><span class="sxs-lookup"><span data-stu-id="0b292-184">Response</span></span>

<span data-ttu-id="0b292-185">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0b292-185">The following is an example of the response.</span></span>

> <span data-ttu-id="0b292-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0b292-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.office365ActiveUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.office365ActiveUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "office365": 1718, 
      "exchange": 1429, 
      "oneDrive": 350, 
      "sharePoint": 795, 
      "skypeForBusiness": 251, 
      "yammer": 47, 
      "teams": 10, 
      "reportDate": "2017-08-29", 
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
