---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: bbb4bda517c70180c35768fd9560c55809b836fe
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35446365"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="21e8a-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="21e8a-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21e8a-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="21e8a-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="21e8a-105">权限</span><span class="sxs-lookup"><span data-stu-id="21e8a-105">Permissions</span></span>

<span data-ttu-id="21e8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="21e8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="21e8a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="21e8a-108">Permission type</span></span>                        | <span data-ttu-id="21e8a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="21e8a-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="21e8a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="21e8a-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="21e8a-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21e8a-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="21e8a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="21e8a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="21e8a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="21e8a-113">Not supported.</span></span>                           |
| <span data-ttu-id="21e8a-114">应用</span><span class="sxs-lookup"><span data-stu-id="21e8a-114">Application</span></span>                            | <span data-ttu-id="21e8a-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="21e8a-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="21e8a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="21e8a-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="21e8a-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="21e8a-117">Function parameters</span></span>

<span data-ttu-id="21e8a-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="21e8a-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="21e8a-119">参数</span><span class="sxs-lookup"><span data-stu-id="21e8a-119">Parameter</span></span> | <span data-ttu-id="21e8a-120">类型</span><span class="sxs-lookup"><span data-stu-id="21e8a-120">Type</span></span>   | <span data-ttu-id="21e8a-121">说明</span><span class="sxs-lookup"><span data-stu-id="21e8a-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="21e8a-122">period</span><span class="sxs-lookup"><span data-stu-id="21e8a-122">period</span></span>    | <span data-ttu-id="21e8a-123">string</span><span class="sxs-lookup"><span data-stu-id="21e8a-123">string</span></span> | <span data-ttu-id="21e8a-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="21e8a-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="21e8a-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="21e8a-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="21e8a-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="21e8a-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="21e8a-127">date</span><span class="sxs-lookup"><span data-stu-id="21e8a-127">date</span></span>      | <span data-ttu-id="21e8a-128">Date</span><span class="sxs-lookup"><span data-stu-id="21e8a-128">Date</span></span>   | <span data-ttu-id="21e8a-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="21e8a-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="21e8a-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="21e8a-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="21e8a-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="21e8a-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="21e8a-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="21e8a-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="21e8a-133">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="21e8a-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="21e8a-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="21e8a-134">The default output type is text/csv.</span></span> <span data-ttu-id="21e8a-135">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="21e8a-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="21e8a-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="21e8a-136">Request headers</span></span>

| <span data-ttu-id="21e8a-137">名称</span><span class="sxs-lookup"><span data-stu-id="21e8a-137">Name</span></span>          | <span data-ttu-id="21e8a-138">说明</span><span class="sxs-lookup"><span data-stu-id="21e8a-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="21e8a-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="21e8a-139">Authorization</span></span> | <span data-ttu-id="21e8a-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="21e8a-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="21e8a-142">响应</span><span class="sxs-lookup"><span data-stu-id="21e8a-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="21e8a-143">CSV</span><span class="sxs-lookup"><span data-stu-id="21e8a-143">CSV</span></span>

<span data-ttu-id="21e8a-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="21e8a-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="21e8a-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="21e8a-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="21e8a-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="21e8a-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="21e8a-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="21e8a-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="21e8a-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="21e8a-148">Report Refresh Date</span></span>
- <span data-ttu-id="21e8a-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="21e8a-149">User Principal Name</span></span>
- <span data-ttu-id="21e8a-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="21e8a-150">Last Activity Date</span></span>
- <span data-ttu-id="21e8a-151">已删除</span><span class="sxs-lookup"><span data-stu-id="21e8a-151">Is Deleted</span></span>
- <span data-ttu-id="21e8a-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="21e8a-152">Deleted Date</span></span>
- <span data-ttu-id="21e8a-153">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="21e8a-153">Used Web</span></span>
- <span data-ttu-id="21e8a-154">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="21e8a-154">Used Windows Phone</span></span>
- <span data-ttu-id="21e8a-155">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="21e8a-155">Used iOS</span></span>
- <span data-ttu-id="21e8a-156">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="21e8a-156">Used Mac</span></span>
- <span data-ttu-id="21e8a-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="21e8a-157">Used Android Phone</span></span>
- <span data-ttu-id="21e8a-158">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="21e8a-158">Used Windows</span></span>
- <span data-ttu-id="21e8a-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="21e8a-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="21e8a-160">JSON</span><span class="sxs-lookup"><span data-stu-id="21e8a-160">JSON</span></span>

<span data-ttu-id="21e8a-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="21e8a-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="21e8a-162">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="21e8a-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="21e8a-163">示例</span><span class="sxs-lookup"><span data-stu-id="21e8a-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="21e8a-164">CSV</span><span class="sxs-lookup"><span data-stu-id="21e8a-164">CSV</span></span>

<span data-ttu-id="21e8a-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="21e8a-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="21e8a-166">请求</span><span class="sxs-lookup"><span data-stu-id="21e8a-166">Request</span></span>

<span data-ttu-id="21e8a-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21e8a-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="21e8a-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="21e8a-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21e8a-169">C#</span><span class="sxs-lookup"><span data-stu-id="21e8a-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21e8a-170">Javascript</span><span class="sxs-lookup"><span data-stu-id="21e8a-170">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21e8a-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="21e8a-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21e8a-172">响应</span><span class="sxs-lookup"><span data-stu-id="21e8a-172">Response</span></span>

<span data-ttu-id="21e8a-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="21e8a-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="21e8a-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="21e8a-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Last Activity Date,Is Deleted,Deleted Date,Used Web,Used Windows Phone,Used iOS,Used Mac,Used Android Phone,Used Windows,Report Period
```

### <a name="json"></a><span data-ttu-id="21e8a-175">JSON</span><span class="sxs-lookup"><span data-stu-id="21e8a-175">JSON</span></span>

<span data-ttu-id="21e8a-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="21e8a-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="21e8a-177">请求</span><span class="sxs-lookup"><span data-stu-id="21e8a-177">Request</span></span>

<span data-ttu-id="21e8a-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="21e8a-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="21e8a-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="21e8a-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="21e8a-180">C#</span><span class="sxs-lookup"><span data-stu-id="21e8a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="21e8a-181">Javascript</span><span class="sxs-lookup"><span data-stu-id="21e8a-181">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="21e8a-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="21e8a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="21e8a-183">响应</span><span class="sxs-lookup"><span data-stu-id="21e8a-183">Response</span></span>

<span data-ttu-id="21e8a-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="21e8a-184">The following is an example of the response.</span></span>

> <span data-ttu-id="21e8a-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="21e8a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsDeviceUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 374

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.teamsDeviceUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "lastActivityDate": "2017-09-01", 
      "isDeleted": false, 
      "deletedDate": null, 
      "usedWeb": false, 
      "usedWindowsPhone": false, 
      "usediOS": true, 
      "usedMac": false, 
      "usedAndroidPhone": false, 
      "usedWindows": true, 
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
