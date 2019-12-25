---
title: 'reportRoot: getSkypeForBusinessActivityUserCounts'
description: 获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。 报表还包含对等会话数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 310b531b90d785917fed836b0b47ffd281ce0a5a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867391"
---
# <a name="reportroot-getskypeforbusinessactivityusercounts"></a><span data-ttu-id="a8bc7-104">reportRoot: getSkypeForBusinessActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="a8bc7-104">reportRoot: getSkypeForBusinessActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8bc7-105">获取通过 Skype for Business 组织并参与在组织中召开的会议会话的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-105">Get the trends on how many unique users organized and participated in conference sessions held in your organization through Skype for Business.</span></span> <span data-ttu-id="a8bc7-106">报表还包含对等会话数。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-106">The report also includes the number of peer-to-peer sessions.</span></span>

> <span data-ttu-id="a8bc7-107">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Skype for Business 活动](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424)。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-107">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business activity](https://support.office.com/client/Skype-for-Business-Online-activity-8cbe2eb2-1194-4fd7-b1ee-9f9287c82424).</span></span>

## <a name="permissions"></a><span data-ttu-id="a8bc7-108">权限</span><span class="sxs-lookup"><span data-stu-id="a8bc7-108">Permissions</span></span>

<span data-ttu-id="a8bc7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a8bc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8bc7-111">Permission type</span></span>                        | <span data-ttu-id="a8bc7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a8bc7-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="a8bc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8bc7-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8bc7-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bc7-114">Reports.Read.All</span></span>                         |
| <span data-ttu-id="a8bc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8bc7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8bc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-116">Not supported.</span></span>                           |
| <span data-ttu-id="a8bc7-117">应用</span><span class="sxs-lookup"><span data-stu-id="a8bc7-117">Application</span></span>                            | <span data-ttu-id="a8bc7-118">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a8bc7-118">Reports.Read.All</span></span>                         |

<span data-ttu-id="a8bc7-119">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-119">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="a8bc7-120">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-120">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="a8bc7-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8bc7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="a8bc7-122">函数参数</span><span class="sxs-lookup"><span data-stu-id="a8bc7-122">Function parameters</span></span>

<span data-ttu-id="a8bc7-123">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-123">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="a8bc7-124">参数</span><span class="sxs-lookup"><span data-stu-id="a8bc7-124">Parameter</span></span> | <span data-ttu-id="a8bc7-125">类型</span><span class="sxs-lookup"><span data-stu-id="a8bc7-125">Type</span></span>   | <span data-ttu-id="a8bc7-126">说明</span><span class="sxs-lookup"><span data-stu-id="a8bc7-126">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="a8bc7-127">period</span><span class="sxs-lookup"><span data-stu-id="a8bc7-127">period</span></span>    | <span data-ttu-id="a8bc7-128">string</span><span class="sxs-lookup"><span data-stu-id="a8bc7-128">string</span></span> | <span data-ttu-id="a8bc7-129">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-129">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="a8bc7-130">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-130">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="a8bc7-131">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-131">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="a8bc7-132">必需。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-132">Required.</span></span> |

<span data-ttu-id="a8bc7-133">此方法支持使用 `$format` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-133">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="a8bc7-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-134">The default output type is text/csv.</span></span> <span data-ttu-id="a8bc7-135">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8bc7-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8bc7-136">Request headers</span></span>

| <span data-ttu-id="a8bc7-137">名称</span><span class="sxs-lookup"><span data-stu-id="a8bc7-137">Name</span></span>          | <span data-ttu-id="a8bc7-138">说明</span><span class="sxs-lookup"><span data-stu-id="a8bc7-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="a8bc7-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8bc7-139">Authorization</span></span> | <span data-ttu-id="a8bc7-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-p107">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="a8bc7-142">响应</span><span class="sxs-lookup"><span data-stu-id="a8bc7-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="a8bc7-143">CSV</span><span class="sxs-lookup"><span data-stu-id="a8bc7-143">CSV</span></span>

<span data-ttu-id="a8bc7-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="a8bc7-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="a8bc7-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="a8bc7-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="a8bc7-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="a8bc7-148">Report Refresh Date</span></span>
- <span data-ttu-id="a8bc7-149">报表日期</span><span class="sxs-lookup"><span data-stu-id="a8bc7-149">Report Date</span></span>
- <span data-ttu-id="a8bc7-150">报表周期</span><span class="sxs-lookup"><span data-stu-id="a8bc7-150">Report Period</span></span>
- <span data-ttu-id="a8bc7-151">对等</span><span class="sxs-lookup"><span data-stu-id="a8bc7-151">Peer-to-peer</span></span>
- <span data-ttu-id="a8bc7-152">组织</span><span class="sxs-lookup"><span data-stu-id="a8bc7-152">Organized</span></span>
- <span data-ttu-id="a8bc7-153">参与</span><span class="sxs-lookup"><span data-stu-id="a8bc7-153">Participated</span></span>

### <a name="json"></a><span data-ttu-id="a8bc7-154">JSON</span><span class="sxs-lookup"><span data-stu-id="a8bc7-154">JSON</span></span>

<span data-ttu-id="a8bc7-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-155">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessActivityUserCounts](../resources/skypeforbusinessactivityusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8bc7-156">示例</span><span class="sxs-lookup"><span data-stu-id="a8bc7-156">Example</span></span>

### <a name="csv"></a><span data-ttu-id="a8bc7-157">CSV</span><span class="sxs-lookup"><span data-stu-id="a8bc7-157">CSV</span></span>

<span data-ttu-id="a8bc7-158">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-158">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="a8bc7-159">请求</span><span class="sxs-lookup"><span data-stu-id="a8bc7-159">Request</span></span>

<span data-ttu-id="a8bc7-160">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-160">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8bc7-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8bc7-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8bc7-162">C#</span><span class="sxs-lookup"><span data-stu-id="a8bc7-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8bc7-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8bc7-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8bc7-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8bc7-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8bc7-165">响应</span><span class="sxs-lookup"><span data-stu-id="a8bc7-165">Response</span></span>

<span data-ttu-id="a8bc7-166">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-166">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="a8bc7-167">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-167">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Report Date,Report Period,Peer-to-peer,Organized,Participated
```

### <a name="json"></a><span data-ttu-id="a8bc7-168">JSON</span><span class="sxs-lookup"><span data-stu-id="a8bc7-168">JSON</span></span>

<span data-ttu-id="a8bc7-169">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-169">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="a8bc7-170">请求</span><span class="sxs-lookup"><span data-stu-id="a8bc7-170">Request</span></span>

<span data-ttu-id="a8bc7-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-171">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="a8bc7-172">HTTP</span><span class="sxs-lookup"><span data-stu-id="a8bc7-172">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessactivityusercounts_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessActivityUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a8bc7-173">C#</span><span class="sxs-lookup"><span data-stu-id="a8bc7-173">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessactivityusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a8bc7-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a8bc7-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessactivityusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a8bc7-175">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a8bc7-175">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessactivityusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a8bc7-176">响应</span><span class="sxs-lookup"><span data-stu-id="a8bc7-176">Response</span></span>

<span data-ttu-id="a8bc7-177">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-177">The following is an example of the response.</span></span>

> <span data-ttu-id="a8bc7-p109">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a8bc7-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessActivityUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 266

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessActivityUserCounts)", 
  "value": [
    {
      "peerToPeer": 413, 
      "organized": 30, 
      "participated": 91, 
      "reportRefreshDate": "2017-09-01", 
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
