---
title: 'reportRoot: getYammerActivityCounts'
description: 获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e7177af218a3fb9dfe34d26c19c67e8b2b452fc7
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868910"
---
# <a name="reportroot-getyammeractivitycounts"></a><span data-ttu-id="a9878-103">reportRoot: getYammerActivityCounts</span><span class="sxs-lookup"><span data-stu-id="a9878-103">reportRoot: getYammerActivityCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a9878-104">获取组织中的 Yammer 活动数趋势，具体是以已发布、已阅读和已赞的消息数为依据。</span><span class="sxs-lookup"><span data-stu-id="a9878-104">Get the trends on the amount of Yammer activity in your organization by how many messages were posted, read, and liked.</span></span>

> <span data-ttu-id="a9878-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 活动](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a)。</span><span class="sxs-lookup"><span data-stu-id="a9878-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer Activity](https://support.office.com/client/Yammer-activity-c7c9f938-5b8e-4d52-b1a2-c7c32cb2312a).</span></span>

## <a name="permissions"></a><span data-ttu-id="a9878-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9878-106">Permissions</span></span>

<span data-ttu-id="a9878-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9878-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a9878-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9878-109">Permission type</span></span>                        | <span data-ttu-id="a9878-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9878-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a9878-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9878-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9878-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9878-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a9878-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9878-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9878-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9878-114">Not supported.</span></span>                           |
| <span data-ttu-id="a9878-115">应用</span><span class="sxs-lookup"><span data-stu-id="a9878-115">Application</span></span>                            | <span data-ttu-id="a9878-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a9878-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="a9878-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a9878-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a9878-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a9878-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a9878-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9878-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerActivityCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a9878-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="a9878-120">Function parameters</span></span>

<span data-ttu-id="a9878-121">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a9878-121">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a9878-122">参数</span><span class="sxs-lookup"><span data-stu-id="a9878-122">Parameter</span></span> | <span data-ttu-id="a9878-123">类型</span><span class="sxs-lookup"><span data-stu-id="a9878-123">Type</span></span>   | <span data-ttu-id="a9878-124">说明</span><span class="sxs-lookup"><span data-stu-id="a9878-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a9878-125">period</span><span class="sxs-lookup"><span data-stu-id="a9878-125">period</span></span>    | <span data-ttu-id="a9878-126">string</span><span class="sxs-lookup"><span data-stu-id="a9878-126">string</span></span> | <span data-ttu-id="a9878-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a9878-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a9878-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a9878-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a9878-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a9878-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a9878-130">必需。</span><span class="sxs-lookup"><span data-stu-id="a9878-130">Required.</span></span> |

<span data-ttu-id="a9878-131">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a9878-131">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a9878-132">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a9878-132">The default output type is text/csv.</span></span> <span data-ttu-id="a9878-133">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a9878-133">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a9878-134">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9878-134">Request headers</span></span>

| <span data-ttu-id="a9878-135">名称</span><span class="sxs-lookup"><span data-stu-id="a9878-135">Name</span></span>          | <span data-ttu-id="a9878-136">说明</span><span class="sxs-lookup"><span data-stu-id="a9878-136">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a9878-137">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9878-137">Authorization</span></span> | <span data-ttu-id="a9878-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9878-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a9878-140">响应</span><span class="sxs-lookup"><span data-stu-id="a9878-140">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a9878-141">CSV</span><span class="sxs-lookup"><span data-stu-id="a9878-141">CSV</span></span>

<span data-ttu-id="a9878-142">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a9878-142">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a9878-143">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a9878-143">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a9878-144">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a9878-144">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a9878-145">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a9878-145">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a9878-146">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a9878-146">Report Refresh Date</span></span>
- <span data-ttu-id="a9878-147">已赞</span><span class="sxs-lookup"><span data-stu-id="a9878-147">Liked</span></span>
- <span data-ttu-id="a9878-148">已发布</span><span class="sxs-lookup"><span data-stu-id="a9878-148">Posted</span></span>
- <span data-ttu-id="a9878-149">已阅读</span><span class="sxs-lookup"><span data-stu-id="a9878-149">Read</span></span>
- <span data-ttu-id="a9878-150">报表日期</span><span class="sxs-lookup"><span data-stu-id="a9878-150">Report Date</span></span>
- <span data-ttu-id="a9878-151">报表周期</span><span class="sxs-lookup"><span data-stu-id="a9878-151">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="a9878-152">JSON</span><span class="sxs-lookup"><span data-stu-id="a9878-152">JSON</span></span>

<span data-ttu-id="a9878-153">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[yammerActivitySummary](../resources/yammeractivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a9878-153">If successful, this method returns a `200 OK` response code and a **[yammerActivitySummary](../resources/yammeractivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9878-154">示例</span><span class="sxs-lookup"><span data-stu-id="a9878-154">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a9878-155">CSV</span><span class="sxs-lookup"><span data-stu-id="a9878-155">CSV</span></span>

<span data-ttu-id="a9878-156">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a9878-156">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a9878-157">请求</span><span class="sxs-lookup"><span data-stu-id="a9878-157">Request</span></span>

<span data-ttu-id="a9878-158">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9878-158">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a9878-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9878-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9878-160">C#</span><span class="sxs-lookup"><span data-stu-id="a9878-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9878-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9878-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9878-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9878-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9878-163">响应</span><span class="sxs-lookup"><span data-stu-id="a9878-163">Response</span></span>

<span data-ttu-id="a9878-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a9878-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a9878-165">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a9878-165">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="a9878-166">JSON</span><span class="sxs-lookup"><span data-stu-id="a9878-166">JSON</span></span>

<span data-ttu-id="a9878-167">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a9878-167">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a9878-168">请求</span><span class="sxs-lookup"><span data-stu-id="a9878-168">Request</span></span>

<span data-ttu-id="a9878-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a9878-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a9878-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="a9878-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammeractivitycounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerActivityCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a9878-171">C#</span><span class="sxs-lookup"><span data-stu-id="a9878-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammeractivitycounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a9878-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a9878-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammeractivitycounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a9878-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a9878-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammeractivitycounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a9878-174">响应</span><span class="sxs-lookup"><span data-stu-id="a9878-174">Response</span></span>

<span data-ttu-id="a9878-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9878-175">The following is an example of the response.</span></span>

> <span data-ttu-id="a9878-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a9878-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "liked": 47, 
      "posted": 59, 
      "read": 986, 
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
