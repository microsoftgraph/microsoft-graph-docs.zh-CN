---
title: 'reportRoot: getYammerDeviceUsageUserDetail function'
description: 获取用户的 Yammer 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: b6ff91494d7f996a1e1a851ccc0ef4d94b842a54
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36722648"
---
# <a name="reportroot-getyammerdeviceusageuserdetail-function"></a><span data-ttu-id="73842-103">reportRoot: getYammerDeviceUsageUserDetail function</span><span class="sxs-lookup"><span data-stu-id="73842-103">reportRoot: getYammerDeviceUsageUserDetail function</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73842-104">获取用户的 Yammer 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="73842-104">Get details about Yammer device usage by user.</span></span>

> <span data-ttu-id="73842-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - Yammer 设备使用情况](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38)。</span><span class="sxs-lookup"><span data-stu-id="73842-105">**Note:** For details about different report views and names, see [Office 365 Reports - Yammer device usage](https://support.office.com/client/Yammer-device-usage-b793ffdd-effa-43d0-849a-b1ca2e899f38).</span></span>

## <a name="permissions"></a><span data-ttu-id="73842-106">权限</span><span class="sxs-lookup"><span data-stu-id="73842-106">Permissions</span></span>

<span data-ttu-id="73842-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="73842-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="73842-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="73842-109">Permission type</span></span>                        | <span data-ttu-id="73842-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="73842-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="73842-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73842-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="73842-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="73842-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="73842-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73842-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="73842-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73842-114">Not supported.</span></span>                           |
| <span data-ttu-id="73842-115">应用</span><span class="sxs-lookup"><span data-stu-id="73842-115">Application</span></span>                            | <span data-ttu-id="73842-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="73842-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="73842-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73842-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getYammerDeviceUsageUserDetail(period='{period_value}')
GET /reports/getYammerDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="73842-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="73842-118">Function parameters</span></span>

<span data-ttu-id="73842-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="73842-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="73842-120">参数</span><span class="sxs-lookup"><span data-stu-id="73842-120">Parameter</span></span> | <span data-ttu-id="73842-121">类型</span><span class="sxs-lookup"><span data-stu-id="73842-121">Type</span></span>   | <span data-ttu-id="73842-122">说明</span><span class="sxs-lookup"><span data-stu-id="73842-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="73842-123">period</span><span class="sxs-lookup"><span data-stu-id="73842-123">period</span></span>    | <span data-ttu-id="73842-124">string</span><span class="sxs-lookup"><span data-stu-id="73842-124">string</span></span> | <span data-ttu-id="73842-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="73842-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="73842-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="73842-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="73842-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="73842-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="73842-128">date</span><span class="sxs-lookup"><span data-stu-id="73842-128">date</span></span>      | <span data-ttu-id="73842-129">Date</span><span class="sxs-lookup"><span data-stu-id="73842-129">Date</span></span>   | <span data-ttu-id="73842-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="73842-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="73842-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="73842-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="73842-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="73842-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="73842-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="73842-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="73842-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="73842-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="73842-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="73842-135">The default output type is text/csv.</span></span> <span data-ttu-id="73842-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="73842-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="73842-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="73842-137">Request headers</span></span>

| <span data-ttu-id="73842-138">名称</span><span class="sxs-lookup"><span data-stu-id="73842-138">Name</span></span>          | <span data-ttu-id="73842-139">说明</span><span class="sxs-lookup"><span data-stu-id="73842-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="73842-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="73842-140">Authorization</span></span> | <span data-ttu-id="73842-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="73842-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="73842-143">响应</span><span class="sxs-lookup"><span data-stu-id="73842-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="73842-144">CSV</span><span class="sxs-lookup"><span data-stu-id="73842-144">CSV</span></span>

<span data-ttu-id="73842-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="73842-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="73842-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="73842-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="73842-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="73842-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="73842-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="73842-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="73842-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="73842-149">Report Refresh Date</span></span>
- <span data-ttu-id="73842-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="73842-150">User Principal Name</span></span>
- <span data-ttu-id="73842-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="73842-151">Display Name</span></span>
- <span data-ttu-id="73842-152">用户状态</span><span class="sxs-lookup"><span data-stu-id="73842-152">User State</span></span>
- <span data-ttu-id="73842-153">状态更改日期</span><span class="sxs-lookup"><span data-stu-id="73842-153">State Change Date</span></span>
- <span data-ttu-id="73842-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="73842-154">Last Activity Date</span></span>
- <span data-ttu-id="73842-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="73842-155">Used Web</span></span>
- <span data-ttu-id="73842-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="73842-156">Used Windows Phone</span></span>
- <span data-ttu-id="73842-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="73842-157">Used Android Phone</span></span>
- <span data-ttu-id="73842-158">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="73842-158">Used iPhone</span></span>
- <span data-ttu-id="73842-159">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="73842-159">Used iPad</span></span>
- <span data-ttu-id="73842-160">使用的其他设备</span><span class="sxs-lookup"><span data-stu-id="73842-160">Used Others</span></span>
- <span data-ttu-id="73842-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="73842-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="73842-162">JSON</span><span class="sxs-lookup"><span data-stu-id="73842-162">JSON</span></span>

<span data-ttu-id="73842-163">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="73842-163">If successful, this method returns a `200 OK` response code and a **[yammerDeviceUsageUserDetail](../resources/yammerdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="73842-164">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="73842-164">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="73842-165">示例</span><span class="sxs-lookup"><span data-stu-id="73842-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="73842-166">CSV</span><span class="sxs-lookup"><span data-stu-id="73842-166">CSV</span></span>

<span data-ttu-id="73842-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="73842-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="73842-168">请求</span><span class="sxs-lookup"><span data-stu-id="73842-168">Request</span></span>

<span data-ttu-id="73842-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73842-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73842-170">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="73842-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73842-171">C#</span><span class="sxs-lookup"><span data-stu-id="73842-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73842-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73842-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73842-173">目标-C</span><span class="sxs-lookup"><span data-stu-id="73842-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73842-174">响应</span><span class="sxs-lookup"><span data-stu-id="73842-174">Response</span></span>

<span data-ttu-id="73842-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="73842-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="73842-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="73842-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,User State,State Change Date,Last Activity Date,Used Web,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Used Others,Report Period
```

### <a name="json"></a><span data-ttu-id="73842-177">JSON</span><span class="sxs-lookup"><span data-stu-id="73842-177">JSON</span></span>

<span data-ttu-id="73842-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="73842-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="73842-179">请求</span><span class="sxs-lookup"><span data-stu-id="73842-179">Request</span></span>

<span data-ttu-id="73842-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="73842-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="73842-181">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="73842-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getyammerdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getYammerDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="73842-182">C#</span><span class="sxs-lookup"><span data-stu-id="73842-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getyammerdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="73842-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="73842-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getyammerdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="73842-184">目标-C</span><span class="sxs-lookup"><span data-stu-id="73842-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getyammerdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="73842-185">响应</span><span class="sxs-lookup"><span data-stu-id="73842-185">Response</span></span>

<span data-ttu-id="73842-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="73842-186">The following is an example of the response.</span></span>

> <span data-ttu-id="73842-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="73842-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.yammerDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 442

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.yammerDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-06", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "userState": "active", 
      "stateChangeDate": "2012-06-26", 
      "lastActivityDate": "2017-09-06", 
      "usedWeb": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "usedOthers": false, 
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
