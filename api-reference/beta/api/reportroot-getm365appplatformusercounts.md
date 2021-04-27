---
title: reportRoot： getM365AppPlatformUserCounts
description: 获取一个报告，该报告提供组织中每个平台的所有应用（Windows、Mac、Web 和移动）的活动用户趋势。
localization_priority: Normal
ms.prod: reports
author: sarahwxy
doc_type: apiPageType
ms.openlocfilehash: 2f6377776cedc7394c2e9573c24e5209d7dda755
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050946"
---
# <a name="reportroot-getm365appplatformusercounts"></a><span data-ttu-id="39287-103">reportRoot： getM365AppPlatformUserCounts</span><span class="sxs-lookup"><span data-stu-id="39287-103">reportRoot: getM365AppPlatformUserCounts</span></span>

<span data-ttu-id="39287-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39287-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39287-105">获取一个报告，该报告提供组织中每个平台的所有应用（Windows、Mac、Web 和移动）的活动用户趋势。</span><span class="sxs-lookup"><span data-stu-id="39287-105">Get a report that provides the trend of active users across all apps for each platform – Windows, Mac, web, and mobile - in your organization.</span></span>

> <span data-ttu-id="39287-106">**注意：** 有关不同报表视图和名称的详细信息，请参阅Microsoft 365 [报表 -](/microsoft-365/admin/activity-reports/microsoft365-apps-usage)Microsoft 365 应用版使用情况。</span><span class="sxs-lookup"><span data-stu-id="39287-106">**Note:** For details about different report views and names, see [Microsoft 365 reports - Microsoft 365 Apps usage](/microsoft-365/admin/activity-reports/microsoft365-apps-usage).</span></span>

## <a name="permissions"></a><span data-ttu-id="39287-107">权限</span><span class="sxs-lookup"><span data-stu-id="39287-107">Permissions</span></span>

<span data-ttu-id="39287-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="39287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="39287-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="39287-110">Permission type</span></span>                        | <span data-ttu-id="39287-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="39287-111">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="39287-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39287-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="39287-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39287-113">Reports.Read.All</span></span>                            |
| <span data-ttu-id="39287-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39287-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39287-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="39287-115">Not supported.</span></span>                              |
| <span data-ttu-id="39287-116">应用</span><span class="sxs-lookup"><span data-stu-id="39287-116">Application</span></span>                            | <span data-ttu-id="39287-117">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="39287-117">Reports.Read.All</span></span>                            |

> <span data-ttu-id="39287-118">**注意：** 对于允许应用代表用户读取服务使用情况报表的委派权限，租户管理员必须为用户分配适当的 Azure AD 受限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="39287-118">**Note:** For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="39287-119">有关详细信息，请参阅[授权 API 读取Microsoft 365使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="39287-119">For details, see [Authorization for APIs to read Microsoft 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="39287-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39287-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getM365AppPlatformUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="39287-121">函数参数</span><span class="sxs-lookup"><span data-stu-id="39287-121">Function parameters</span></span>

<span data-ttu-id="39287-122">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="39287-122">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="39287-123">参数</span><span class="sxs-lookup"><span data-stu-id="39287-123">Parameter</span></span> | <span data-ttu-id="39287-124">类型</span><span class="sxs-lookup"><span data-stu-id="39287-124">Type</span></span>   | <span data-ttu-id="39287-125">说明</span><span class="sxs-lookup"><span data-stu-id="39287-125">Description</span></span>                                                                                                                                                                                                                                                       |
| :-------- | :----- | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="39287-126">period</span><span class="sxs-lookup"><span data-stu-id="39287-126">period</span></span>    | <span data-ttu-id="39287-127">string</span><span class="sxs-lookup"><span data-stu-id="39287-127">string</span></span> | <span data-ttu-id="39287-128">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="39287-128">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="39287-129">{period_value} 支持的值是 `D7` `D30` ：、、 `D90` 和 `D180` 。</span><span class="sxs-lookup"><span data-stu-id="39287-129">The supported values for {period_value} are: `D7`, `D30`, `D90`, and `D180`.</span></span> <span data-ttu-id="39287-130">这些值采用格式 D *n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="39287-130">These values follow the format D *n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="39287-131">必需。</span><span class="sxs-lookup"><span data-stu-id="39287-131">Required.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="39287-132">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="39287-132">Optional query parameters</span></span>

<span data-ttu-id="39287-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="39287-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="39287-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="39287-134">The default output type is text/csv.</span></span> <span data-ttu-id="39287-135">但是，如果要指定输出类型，可以使用 OData 查询参数将默认输出设置为 `$format` text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="39287-135">However, if you want to specify the output type, you can use the OData `$format` query parameter to set the default output to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="39287-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="39287-136">Request headers</span></span>

| <span data-ttu-id="39287-137">名称</span><span class="sxs-lookup"><span data-stu-id="39287-137">Name</span></span>          | <span data-ttu-id="39287-138">说明</span><span class="sxs-lookup"><span data-stu-id="39287-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="39287-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="39287-139">Authorization</span></span> | <span data-ttu-id="39287-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="39287-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="39287-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="39287-142">Request body</span></span>

<span data-ttu-id="39287-143">请勿为此方法提供请求正文。</span><span class="sxs-lookup"><span data-stu-id="39287-143">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="39287-144">响应</span><span class="sxs-lookup"><span data-stu-id="39287-144">Response</span></span>

<span data-ttu-id="39287-145">如果成功，此方法在响应 `200 OK` 正文中返回 响应[](../resources/intune-shared-report.md)代码和 report 对象。</span><span class="sxs-lookup"><span data-stu-id="39287-145">If successful, this method returns a `200 OK` response code and a [report](../resources/intune-shared-report.md) object in the response body.</span></span> <span data-ttu-id="39287-146">报表数据包含在 **报表对象的 content\*\*\*\*属性中**。</span><span class="sxs-lookup"><span data-stu-id="39287-146">Report data is contained in the **content** property of the **report** object.</span></span>

### <a name="csv"></a><span data-ttu-id="39287-147">CSV</span><span class="sxs-lookup"><span data-stu-id="39287-147">CSV</span></span>

<span data-ttu-id="39287-148">如果成功，请求 **content** 属性将返回响应，该响应会重定向到报告的预先验证的 `302 Found` 下载 URL。</span><span class="sxs-lookup"><span data-stu-id="39287-148">If successful, requesting the **content** property returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="39287-149">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="39287-149">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="39287-150">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 标头。</span><span class="sxs-lookup"><span data-stu-id="39287-150">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="39287-151">CSV 文件包含下面的列标题：</span><span class="sxs-lookup"><span data-stu-id="39287-151">The CSV file has the following headers for columns:</span></span>

- <span data-ttu-id="39287-152">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="39287-152">Report Refresh Date</span></span>
- <span data-ttu-id="39287-153">报表周期</span><span class="sxs-lookup"><span data-stu-id="39287-153">Report Period</span></span>
- <span data-ttu-id="39287-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="39287-154">Report Date</span></span>
- <span data-ttu-id="39287-155">Outlook</span><span class="sxs-lookup"><span data-stu-id="39287-155">Outlook</span></span>
- <span data-ttu-id="39287-156">Word</span><span class="sxs-lookup"><span data-stu-id="39287-156">Word</span></span>
- <span data-ttu-id="39287-157">Excel</span><span class="sxs-lookup"><span data-stu-id="39287-157">Excel</span></span>
- <span data-ttu-id="39287-158">PowerPoint</span><span class="sxs-lookup"><span data-stu-id="39287-158">PowerPoint</span></span>
- <span data-ttu-id="39287-159">OneNote</span><span class="sxs-lookup"><span data-stu-id="39287-159">OneNote</span></span>
- <span data-ttu-id="39287-160">Teams</span><span class="sxs-lookup"><span data-stu-id="39287-160">Teams</span></span>

### <a name="json"></a><span data-ttu-id="39287-161">JSON</span><span class="sxs-lookup"><span data-stu-id="39287-161">JSON</span></span>

<span data-ttu-id="39287-162">如果成功，请求 **content** 属性在响应正文中返回 响应代码和 `200 OK` JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="39287-162">If successful, requesting the **content** property returns a `200 OK` response code and a JSON object in response body.</span></span>

## <a name="examples"></a><span data-ttu-id="39287-163">示例</span><span class="sxs-lookup"><span data-stu-id="39287-163">Examples</span></span>

### <a name="example-1-csv-output"></a><span data-ttu-id="39287-164">示例 1：CSV 输出</span><span class="sxs-lookup"><span data-stu-id="39287-164">Example 1: CSV output</span></span>

<span data-ttu-id="39287-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="39287-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="39287-166">请求</span><span class="sxs-lookup"><span data-stu-id="39287-166">Request</span></span>

<span data-ttu-id="39287-167">下面是请求获取 content 属性 **的示例** 。</span><span class="sxs-lookup"><span data-stu-id="39287-167">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="39287-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="39287-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=text/csv
```
# <a name="c"></a>[<span data-ttu-id="39287-169">C#</span><span class="sxs-lookup"><span data-stu-id="39287-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39287-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39287-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39287-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39287-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39287-172">Java</span><span class="sxs-lookup"><span data-stu-id="39287-172">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appplatformusercounts-csv-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="39287-173">响应</span><span class="sxs-lookup"><span data-stu-id="39287-173">Response</span></span>

<span data-ttu-id="39287-174">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39287-174">The following is an example of the response.</span></span>

<!-- { "blockType": "response" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="39287-175">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="39287-175">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Period,Report Date,Windows,Mac,Mobile,Web
```

### <a name="example-2-json-output"></a><span data-ttu-id="39287-176">示例 2：JSON 输出</span><span class="sxs-lookup"><span data-stu-id="39287-176">Example 2: JSON output</span></span>

<span data-ttu-id="39287-177">下面是返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="39287-177">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="39287-178">请求</span><span class="sxs-lookup"><span data-stu-id="39287-178">Request</span></span>

<span data-ttu-id="39287-179">下面是请求获取 content 属性 **的示例** 。</span><span class="sxs-lookup"><span data-stu-id="39287-179">The following is an example of the request to get the **content** property.</span></span>



# <a name="http"></a>[<span data-ttu-id="39287-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="39287-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getM365AppPlatformUserCounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getM365AppPlatformUserCounts(period='D7')/content?$format=application/json
```
# <a name="c"></a>[<span data-ttu-id="39287-181">C#</span><span class="sxs-lookup"><span data-stu-id="39287-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getm365appplatformusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="39287-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="39287-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getm365appplatformusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="39287-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="39287-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getm365appplatformusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="39287-184">Java</span><span class="sxs-lookup"><span data-stu-id="39287-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/reportroot-getm365appplatformusercounts-json-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="39287-185">响应</span><span class="sxs-lookup"><span data-stu-id="39287-185">Response</span></span>

<span data-ttu-id="39287-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="39287-186">The following is an example of the response.</span></span>

> <span data-ttu-id="39287-187">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="39287-187">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 156

{
  "value": [
    {
      "reportRefreshDate": "2020-06-30",
      "reportPeriod": 7,
      "userCounts": [
        {
          "reportDate": "2020-06-30",
          "windows": 1445,
          "mac": 146,
          "mobile": 1131,
          "web": 1080
        }
      ]
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
