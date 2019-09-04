---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 3bc3211a919b460ea69215af1f90a050e58302f1
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36724949"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="c4fce-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="c4fce-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4fce-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="c4fce-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4fce-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4fce-105">Permissions</span></span>

<span data-ttu-id="c4fce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4fce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c4fce-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4fce-108">Permission type</span></span>                        | <span data-ttu-id="c4fce-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4fce-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="c4fce-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4fce-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c4fce-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4fce-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="c4fce-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4fce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4fce-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4fce-113">Not supported.</span></span>                           |
| <span data-ttu-id="c4fce-114">应用</span><span class="sxs-lookup"><span data-stu-id="c4fce-114">Application</span></span>                            | <span data-ttu-id="c4fce-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="c4fce-115">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="c4fce-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4fce-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="c4fce-117">函数参数</span><span class="sxs-lookup"><span data-stu-id="c4fce-117">Function parameters</span></span>

<span data-ttu-id="c4fce-118">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="c4fce-118">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="c4fce-119">参数</span><span class="sxs-lookup"><span data-stu-id="c4fce-119">Parameter</span></span> | <span data-ttu-id="c4fce-120">类型</span><span class="sxs-lookup"><span data-stu-id="c4fce-120">Type</span></span>   | <span data-ttu-id="c4fce-121">说明</span><span class="sxs-lookup"><span data-stu-id="c4fce-121">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="c4fce-122">period</span><span class="sxs-lookup"><span data-stu-id="c4fce-122">period</span></span>    | <span data-ttu-id="c4fce-123">string</span><span class="sxs-lookup"><span data-stu-id="c4fce-123">string</span></span> | <span data-ttu-id="c4fce-124">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c4fce-124">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="c4fce-125">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="c4fce-125">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="c4fce-126">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="c4fce-126">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="c4fce-127">date</span><span class="sxs-lookup"><span data-stu-id="c4fce-127">date</span></span>      | <span data-ttu-id="c4fce-128">Date</span><span class="sxs-lookup"><span data-stu-id="c4fce-128">Date</span></span>   | <span data-ttu-id="c4fce-129">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="c4fce-129">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="c4fce-130">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="c4fce-130">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="c4fce-131">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="c4fce-131">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="c4fce-132">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="c4fce-132">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="c4fce-133">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4fce-133">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="c4fce-134">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="c4fce-134">The default output type is text/csv.</span></span> <span data-ttu-id="c4fce-135">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="c4fce-135">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4fce-136">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4fce-136">Request headers</span></span>

| <span data-ttu-id="c4fce-137">名称</span><span class="sxs-lookup"><span data-stu-id="c4fce-137">Name</span></span>          | <span data-ttu-id="c4fce-138">说明</span><span class="sxs-lookup"><span data-stu-id="c4fce-138">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="c4fce-139">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4fce-139">Authorization</span></span> | <span data-ttu-id="c4fce-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4fce-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="c4fce-142">响应</span><span class="sxs-lookup"><span data-stu-id="c4fce-142">Response</span></span>

### <a name="csv"></a><span data-ttu-id="c4fce-143">CSV</span><span class="sxs-lookup"><span data-stu-id="c4fce-143">CSV</span></span>

<span data-ttu-id="c4fce-144">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="c4fce-144">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="c4fce-145">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="c4fce-145">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="c4fce-146">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="c4fce-146">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="c4fce-147">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="c4fce-147">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="c4fce-148">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="c4fce-148">Report Refresh Date</span></span>
- <span data-ttu-id="c4fce-149">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="c4fce-149">User Principal Name</span></span>
- <span data-ttu-id="c4fce-150">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="c4fce-150">Last Activity Date</span></span>
- <span data-ttu-id="c4fce-151">已删除</span><span class="sxs-lookup"><span data-stu-id="c4fce-151">Is Deleted</span></span>
- <span data-ttu-id="c4fce-152">删除日期</span><span class="sxs-lookup"><span data-stu-id="c4fce-152">Deleted Date</span></span>
- <span data-ttu-id="c4fce-153">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="c4fce-153">Used Web</span></span>
- <span data-ttu-id="c4fce-154">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="c4fce-154">Used Windows Phone</span></span>
- <span data-ttu-id="c4fce-155">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="c4fce-155">Used iOS</span></span>
- <span data-ttu-id="c4fce-156">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="c4fce-156">Used Mac</span></span>
- <span data-ttu-id="c4fce-157">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="c4fce-157">Used Android Phone</span></span>
- <span data-ttu-id="c4fce-158">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="c4fce-158">Used Windows</span></span>
- <span data-ttu-id="c4fce-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="c4fce-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="c4fce-160">JSON</span><span class="sxs-lookup"><span data-stu-id="c4fce-160">JSON</span></span>

<span data-ttu-id="c4fce-161">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="c4fce-161">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="c4fce-162">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="c4fce-162">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="c4fce-163">示例</span><span class="sxs-lookup"><span data-stu-id="c4fce-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="c4fce-164">CSV</span><span class="sxs-lookup"><span data-stu-id="c4fce-164">CSV</span></span>

<span data-ttu-id="c4fce-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4fce-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="c4fce-166">请求</span><span class="sxs-lookup"><span data-stu-id="c4fce-166">Request</span></span>

<span data-ttu-id="c4fce-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4fce-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4fce-168">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c4fce-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4fce-169">C#</span><span class="sxs-lookup"><span data-stu-id="c4fce-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4fce-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4fce-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4fce-171">目标-C</span><span class="sxs-lookup"><span data-stu-id="c4fce-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4fce-172">响应</span><span class="sxs-lookup"><span data-stu-id="c4fce-172">Response</span></span>

<span data-ttu-id="c4fce-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c4fce-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="c4fce-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="c4fce-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="c4fce-175">JSON</span><span class="sxs-lookup"><span data-stu-id="c4fce-175">JSON</span></span>

<span data-ttu-id="c4fce-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="c4fce-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="c4fce-177">请求</span><span class="sxs-lookup"><span data-stu-id="c4fce-177">Request</span></span>

<span data-ttu-id="c4fce-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c4fce-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4fce-179">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c4fce-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4fce-180">C#</span><span class="sxs-lookup"><span data-stu-id="c4fce-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4fce-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4fce-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4fce-182">目标-C</span><span class="sxs-lookup"><span data-stu-id="c4fce-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="c4fce-183">响应</span><span class="sxs-lookup"><span data-stu-id="c4fce-183">Response</span></span>

<span data-ttu-id="c4fce-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c4fce-184">The following is an example of the response.</span></span>

> <span data-ttu-id="c4fce-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c4fce-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
