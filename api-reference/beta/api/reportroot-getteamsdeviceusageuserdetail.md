---
title: 'reportRoot: getTeamsDeviceUsageUserDetail'
description: 按用户获取有关 Microsoft Teams 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: c3758796e5fd5fa2997019e137211b787d5f005b
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868931"
---
# <a name="reportroot-getteamsdeviceusageuserdetail"></a><span data-ttu-id="bd205-103">reportRoot: getTeamsDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="bd205-103">reportRoot: getTeamsDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd205-104">按用户获取有关 Microsoft Teams 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="bd205-104">Get details about Microsoft Teams device usage by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="bd205-105">权限</span><span class="sxs-lookup"><span data-stu-id="bd205-105">Permissions</span></span>

<span data-ttu-id="bd205-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd205-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bd205-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd205-108">Permission type</span></span>                        | <span data-ttu-id="bd205-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd205-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="bd205-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd205-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bd205-111">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd205-111">Reports.Read.All</span></span>                         |
| <span data-ttu-id="bd205-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd205-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bd205-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd205-113">Not supported.</span></span>                           |
| <span data-ttu-id="bd205-114">应用</span><span class="sxs-lookup"><span data-stu-id="bd205-114">Application</span></span>                            | <span data-ttu-id="bd205-115">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="bd205-115">Reports.Read.All</span></span>                         |

<span data-ttu-id="bd205-116">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="bd205-116">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="bd205-117">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="bd205-117">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="bd205-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd205-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /reports/getTeamsDeviceUsageUserDetail(period='D7')
GET /reports/getTeamsDeviceUsageUserDetail(date=2017-09-01)
```

## <a name="function-parameters"></a><span data-ttu-id="bd205-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="bd205-119">Function parameters</span></span>

<span data-ttu-id="bd205-120">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="bd205-120">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="bd205-121">参数</span><span class="sxs-lookup"><span data-stu-id="bd205-121">Parameter</span></span> | <span data-ttu-id="bd205-122">类型</span><span class="sxs-lookup"><span data-stu-id="bd205-122">Type</span></span>   | <span data-ttu-id="bd205-123">说明</span><span class="sxs-lookup"><span data-stu-id="bd205-123">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="bd205-124">period</span><span class="sxs-lookup"><span data-stu-id="bd205-124">period</span></span>    | <span data-ttu-id="bd205-125">string</span><span class="sxs-lookup"><span data-stu-id="bd205-125">string</span></span> | <span data-ttu-id="bd205-126">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bd205-126">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="bd205-127">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="bd205-127">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="bd205-128">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="bd205-128">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="bd205-129">date</span><span class="sxs-lookup"><span data-stu-id="bd205-129">date</span></span>      | <span data-ttu-id="bd205-130">Date</span><span class="sxs-lookup"><span data-stu-id="bd205-130">Date</span></span>   | <span data-ttu-id="bd205-131">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="bd205-131">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="bd205-132">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="bd205-132">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="bd205-133">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="bd205-133">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="bd205-134">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="bd205-134">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="bd205-135">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bd205-135">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="bd205-136">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="bd205-136">The default output type is text/csv.</span></span> <span data-ttu-id="bd205-137">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="bd205-137">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bd205-138">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd205-138">Request headers</span></span>

| <span data-ttu-id="bd205-139">名称</span><span class="sxs-lookup"><span data-stu-id="bd205-139">Name</span></span>          | <span data-ttu-id="bd205-140">说明</span><span class="sxs-lookup"><span data-stu-id="bd205-140">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="bd205-141">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd205-141">Authorization</span></span> | <span data-ttu-id="bd205-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bd205-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="bd205-144">响应</span><span class="sxs-lookup"><span data-stu-id="bd205-144">Response</span></span>

### <a name="csv"></a><span data-ttu-id="bd205-145">CSV</span><span class="sxs-lookup"><span data-stu-id="bd205-145">CSV</span></span>

<span data-ttu-id="bd205-146">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="bd205-146">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="bd205-147">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="bd205-147">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="bd205-148">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="bd205-148">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="bd205-149">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="bd205-149">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="bd205-150">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="bd205-150">Report Refresh Date</span></span>
- <span data-ttu-id="bd205-151">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bd205-151">User Principal Name</span></span>
- <span data-ttu-id="bd205-152">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="bd205-152">Last Activity Date</span></span>
- <span data-ttu-id="bd205-153">已删除</span><span class="sxs-lookup"><span data-stu-id="bd205-153">Is Deleted</span></span>
- <span data-ttu-id="bd205-154">删除日期</span><span class="sxs-lookup"><span data-stu-id="bd205-154">Deleted Date</span></span>
- <span data-ttu-id="bd205-155">使用的 Web</span><span class="sxs-lookup"><span data-stu-id="bd205-155">Used Web</span></span>
- <span data-ttu-id="bd205-156">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="bd205-156">Used Windows Phone</span></span>
- <span data-ttu-id="bd205-157">使用的 iOS</span><span class="sxs-lookup"><span data-stu-id="bd205-157">Used iOS</span></span>
- <span data-ttu-id="bd205-158">使用的 Mac</span><span class="sxs-lookup"><span data-stu-id="bd205-158">Used Mac</span></span>
- <span data-ttu-id="bd205-159">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="bd205-159">Used Android Phone</span></span>
- <span data-ttu-id="bd205-160">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="bd205-160">Used Windows</span></span>
- <span data-ttu-id="bd205-161">报表周期</span><span class="sxs-lookup"><span data-stu-id="bd205-161">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="bd205-162">JSON</span><span class="sxs-lookup"><span data-stu-id="bd205-162">JSON</span></span>

<span data-ttu-id="bd205-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="bd205-163">If successful, this method returns a `200 OK` response code and a **[teamsDeviceUsageUserDetail](../resources/teamsdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="bd205-164">此请求的默认页面大小为2000个项目。</span><span class="sxs-lookup"><span data-stu-id="bd205-164">The default page size for this request is 2000 items.</span></span>

## <a name="example"></a><span data-ttu-id="bd205-165">示例</span><span class="sxs-lookup"><span data-stu-id="bd205-165">Example</span></span>

### <a name="csv"></a><span data-ttu-id="bd205-166">CSV</span><span class="sxs-lookup"><span data-stu-id="bd205-166">CSV</span></span>

<span data-ttu-id="bd205-167">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="bd205-167">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="bd205-168">请求</span><span class="sxs-lookup"><span data-stu-id="bd205-168">Request</span></span>

<span data-ttu-id="bd205-169">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd205-169">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bd205-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd205-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd205-171">C#</span><span class="sxs-lookup"><span data-stu-id="bd205-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd205-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd205-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd205-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd205-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd205-174">响应</span><span class="sxs-lookup"><span data-stu-id="bd205-174">Response</span></span>

<span data-ttu-id="bd205-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bd205-175">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="bd205-176">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="bd205-176">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="bd205-177">JSON</span><span class="sxs-lookup"><span data-stu-id="bd205-177">JSON</span></span>

<span data-ttu-id="bd205-178">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="bd205-178">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="bd205-179">请求</span><span class="sxs-lookup"><span data-stu-id="bd205-179">Request</span></span>

<span data-ttu-id="bd205-180">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bd205-180">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bd205-181">HTTP</span><span class="sxs-lookup"><span data-stu-id="bd205-181">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getteamsdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getTeamsDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bd205-182">C#</span><span class="sxs-lookup"><span data-stu-id="bd205-182">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getteamsdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bd205-183">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bd205-183">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getteamsdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bd205-184">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bd205-184">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getteamsdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="bd205-185">响应</span><span class="sxs-lookup"><span data-stu-id="bd205-185">Response</span></span>

<span data-ttu-id="bd205-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bd205-186">The following is an example of the response.</span></span>

> <span data-ttu-id="bd205-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bd205-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
