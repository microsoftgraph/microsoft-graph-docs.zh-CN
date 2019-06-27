---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: 获取用户的 Skype for Business 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: da944ff01b6bc537ab8c1ebc822197f836df7985
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265238"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="e780e-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="e780e-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e780e-104">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="e780e-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="e780e-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="e780e-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="e780e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e780e-106">Permissions</span></span>

<span data-ttu-id="e780e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e780e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e780e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e780e-109">Permission type</span></span>                        | <span data-ttu-id="e780e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e780e-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e780e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e780e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e780e-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e780e-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e780e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e780e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e780e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e780e-114">Not supported.</span></span>                           |
| <span data-ttu-id="e780e-115">应用</span><span class="sxs-lookup"><span data-stu-id="e780e-115">Application</span></span>                            | <span data-ttu-id="e780e-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e780e-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e780e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e780e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="e780e-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="e780e-118">Function parameters</span></span>

<span data-ttu-id="e780e-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e780e-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="e780e-120">参数</span><span class="sxs-lookup"><span data-stu-id="e780e-120">Parameter</span></span> | <span data-ttu-id="e780e-121">类型</span><span class="sxs-lookup"><span data-stu-id="e780e-121">Type</span></span>   | <span data-ttu-id="e780e-122">说明</span><span class="sxs-lookup"><span data-stu-id="e780e-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e780e-123">period</span><span class="sxs-lookup"><span data-stu-id="e780e-123">period</span></span>    | <span data-ttu-id="e780e-124">string</span><span class="sxs-lookup"><span data-stu-id="e780e-124">string</span></span> | <span data-ttu-id="e780e-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e780e-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e780e-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e780e-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e780e-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e780e-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="e780e-128">date</span><span class="sxs-lookup"><span data-stu-id="e780e-128">date</span></span>      | <span data-ttu-id="e780e-129">Date</span><span class="sxs-lookup"><span data-stu-id="e780e-129">Date</span></span>   | <span data-ttu-id="e780e-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="e780e-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="e780e-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="e780e-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="e780e-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="e780e-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="e780e-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="e780e-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="e780e-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e780e-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e780e-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e780e-135">The default output type is text/csv.</span></span> <span data-ttu-id="e780e-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e780e-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e780e-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="e780e-137">Request headers</span></span>

| <span data-ttu-id="e780e-138">名称</span><span class="sxs-lookup"><span data-stu-id="e780e-138">Name</span></span>          | <span data-ttu-id="e780e-139">说明</span><span class="sxs-lookup"><span data-stu-id="e780e-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e780e-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="e780e-140">Authorization</span></span> | <span data-ttu-id="e780e-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e780e-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e780e-143">响应</span><span class="sxs-lookup"><span data-stu-id="e780e-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e780e-144">CSV</span><span class="sxs-lookup"><span data-stu-id="e780e-144">CSV</span></span>

<span data-ttu-id="e780e-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e780e-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e780e-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e780e-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e780e-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e780e-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e780e-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e780e-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e780e-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e780e-149">Report Refresh Date</span></span>
- <span data-ttu-id="e780e-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e780e-150">User Principal Name</span></span>
- <span data-ttu-id="e780e-151">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="e780e-151">Last Activity Date</span></span>
- <span data-ttu-id="e780e-152">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="e780e-152">Used Windows</span></span>
- <span data-ttu-id="e780e-153">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="e780e-153">Used Windows Phone</span></span>
- <span data-ttu-id="e780e-154">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="e780e-154">Used Android Phone</span></span>
- <span data-ttu-id="e780e-155">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="e780e-155">Used iPhone</span></span>
- <span data-ttu-id="e780e-156">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="e780e-156">Used iPad</span></span>
- <span data-ttu-id="e780e-157">报表周期</span><span class="sxs-lookup"><span data-stu-id="e780e-157">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e780e-158">JSON</span><span class="sxs-lookup"><span data-stu-id="e780e-158">JSON</span></span>

<span data-ttu-id="e780e-159">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e780e-159">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="e780e-160">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="e780e-160">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="e780e-161">示例</span><span class="sxs-lookup"><span data-stu-id="e780e-161">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e780e-162">CSV</span><span class="sxs-lookup"><span data-stu-id="e780e-162">CSV</span></span>

<span data-ttu-id="e780e-163">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e780e-163">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e780e-164">请求</span><span class="sxs-lookup"><span data-stu-id="e780e-164">Request</span></span>

<span data-ttu-id="e780e-165">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e780e-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e780e-166">响应</span><span class="sxs-lookup"><span data-stu-id="e780e-166">Response</span></span>

<span data-ttu-id="e780e-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e780e-167">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e780e-168">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e780e-168">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e780e-169">C#</span><span class="sxs-lookup"><span data-stu-id="e780e-169">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e780e-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="e780e-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e780e-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="e780e-171">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e780e-172">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e780e-172">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Used Windows,Used Windows Phone,Used Android Phone,Used iPhone,Used iPad,Report Period
```

### <a name="json"></a><span data-ttu-id="e780e-173">JSON</span><span class="sxs-lookup"><span data-stu-id="e780e-173">JSON</span></span>

<span data-ttu-id="e780e-174">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e780e-174">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e780e-175">请求</span><span class="sxs-lookup"><span data-stu-id="e780e-175">Request</span></span>

<span data-ttu-id="e780e-176">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e780e-176">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e780e-177">响应</span><span class="sxs-lookup"><span data-stu-id="e780e-177">Response</span></span>

<span data-ttu-id="e780e-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e780e-178">The following is an example of the response.</span></span>

> <span data-ttu-id="e780e-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e780e-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.skypeForBusinessDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 356

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.skypeForBusinessDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "usedWindows": true, 
      "usedWindowsPhone": false, 
      "usedAndroidPhone": false, 
      "usediPhone": false, 
      "usediPad": false, 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e780e-181">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e780e-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e780e-182">C#</span><span class="sxs-lookup"><span data-stu-id="e780e-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e780e-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="e780e-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e780e-184">目标-C</span><span class="sxs-lookup"><span data-stu-id="e780e-184">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getskypeforbusinessdeviceusageuserdetail_json-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getskypeforbusinessdeviceusageuserdetail.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
