---
title: 'reportRoot: getYammerActivityUserCounts'
description: 获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 44f80f10dd160855e1d24b5477f9cbeab5d862d1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867076"
---
# <a name="reportroot-getyammeractivityusercounts"></a><span data-ttu-id="fda81-103">reportRoot: getYammerActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="fda81-103">reportRoot: getYammerActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fda81-104">获取已发布、已阅读和已赞 Yammer 消息的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="fda81-104">Get the trends on the number of unique users who posted, read, and liked Yammer messages.</span></span>

> <span data-ttu-id="fda81-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="fda81-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="fda81-106">权限</span><span class="sxs-lookup"><span data-stu-id="fda81-106">Permissions</span></span>

<span data-ttu-id="fda81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fda81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fda81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fda81-109">Permission type</span></span>                        | <span data-ttu-id="fda81-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fda81-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fda81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fda81-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fda81-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fda81-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fda81-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fda81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fda81-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fda81-114">Not supported.</span></span>                           |
| <span data-ttu-id="fda81-115">应用</span><span class="sxs-lookup"><span data-stu-id="fda81-115">Application</span></span>                            | <span data-ttu-id="fda81-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fda81-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="fda81-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="fda81-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="fda81-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="fda81-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="fda81-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fda81-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="fda81-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="fda81-120">Function parameters</span></span>

<span data-ttu-id="fda81-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fda81-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="fda81-122">参数</span><span class="sxs-lookup"><span data-stu-id="fda81-122">Parameter</span></span> | <span data-ttu-id="fda81-123">类型</span><span class="sxs-lookup"><span data-stu-id="fda81-123">Type</span></span>   | <span data-ttu-id="fda81-124">说明</span><span class="sxs-lookup"><span data-stu-id="fda81-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fda81-125">period</span><span class="sxs-lookup"><span data-stu-id="fda81-125">period</span></span>    | <span data-ttu-id="fda81-126">string</span><span class="sxs-lookup"><span data-stu-id="fda81-126">string</span></span> | <span data-ttu-id="fda81-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fda81-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fda81-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fda81-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fda81-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fda81-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="fda81-130">必需。</span><span class="sxs-lookup"><span data-stu-id="fda81-130">Required.</span></span> |

<span data-ttu-id="fda81-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fda81-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fda81-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="fda81-132">The default output type is text/csv.</span></span> <span data-ttu-id="fda81-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="fda81-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fda81-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="fda81-134">Request headers</span></span>

| <span data-ttu-id="fda81-135">名称</span><span class="sxs-lookup"><span data-stu-id="fda81-135">Name</span></span>          | <span data-ttu-id="fda81-136">说明</span><span class="sxs-lookup"><span data-stu-id="fda81-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fda81-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda81-137">Authorization</span></span> | <span data-ttu-id="fda81-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fda81-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fda81-140">响应</span><span class="sxs-lookup"><span data-stu-id="fda81-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fda81-141">CSV</span><span class="sxs-lookup"><span data-stu-id="fda81-141">CSV</span></span>

<span data-ttu-id="fda81-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fda81-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fda81-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fda81-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fda81-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fda81-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fda81-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fda81-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fda81-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fda81-146">Report Refresh Date</span></span>
- <span data-ttu-id="fda81-147">已赞</span><span class="sxs-lookup"><span data-stu-id="fda81-147">Liked</span></span>
- <span data-ttu-id="fda81-148">已发布</span><span class="sxs-lookup"><span data-stu-id="fda81-148">Posted</span></span>
- <span data-ttu-id="fda81-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="fda81-149">Read</span></span>
- <span data-ttu-id="fda81-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="fda81-150">Report Date</span></span>
- <span data-ttu-id="fda81-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="fda81-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fda81-152">JSON</span><span class="sxs-lookup"><span data-stu-id="fda81-152">JSON</span></span>

<span data-ttu-id="fda81-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fda81-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda81-154">示例</span><span class="sxs-lookup"><span data-stu-id="fda81-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fda81-155">CSV</span><span class="sxs-lookup"><span data-stu-id="fda81-155">CSV</span></span>

<span data-ttu-id="fda81-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="fda81-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fda81-157">请求</span><span class="sxs-lookup"><span data-stu-id="fda81-157">Request</span></span>

<span data-ttu-id="fda81-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fda81-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fda81-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="fda81-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fda81-160">C#</span><span class="sxs-lookup"><span data-stu-id="fda81-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fda81-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fda81-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fda81-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fda81-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fda81-163">响应</span><span class="sxs-lookup"><span data-stu-id="fda81-163">Response</span></span>

<span data-ttu-id="fda81-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fda81-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fda81-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fda81-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="fda81-166">JSON</span><span class="sxs-lookup"><span data-stu-id="fda81-166">JSON</span></span>

<span data-ttu-id="fda81-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fda81-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fda81-168">请求</span><span class="sxs-lookup"><span data-stu-id="fda81-168">Request</span></span>

<span data-ttu-id="fda81-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fda81-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fda81-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="fda81-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fda81-171">C#</span><span class="sxs-lookup"><span data-stu-id="fda81-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fda81-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fda81-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fda81-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fda81-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fda81-174">响应</span><span class="sxs-lookup"><span data-stu-id="fda81-174">Response</span></span>

<span data-ttu-id="fda81-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fda81-175">The following is an example of the response.</span></span>

> <span data-ttu-id="fda81-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fda81-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
