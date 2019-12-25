---
title: 'reportRoot: getSkypeForBusinessDeviceUsageUserDetail'
description: 获取用户的 Skype for Business 设备使用情况的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 7e7f4068713c8f71e9f385ce7621ec501c7ae809
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40867373"
---
# <a name="reportroot-getskypeforbusinessdeviceusageuserdetail"></a><span data-ttu-id="3d13a-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="3d13a-103">reportRoot: getSkypeForBusinessDeviceUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d13a-104">获取用户的 Skype for Business 设备使用情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3d13a-104">Get details about Skype for Business device usage by user.</span></span>

> <span data-ttu-id="3d13a-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 已使用的 Skype for Business 客户端](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3)。</span><span class="sxs-lookup"><span data-stu-id="3d13a-105">**Note:** For details about different report views and names, see [Office 365 Reports - Skype for Business clients used](https://support.office.com/client/Skype-for-Business-clients-used-b9019c36-034f-40c7-acb0-c2a0400b03c3).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d13a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3d13a-106">Permissions</span></span>

<span data-ttu-id="3d13a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d13a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3d13a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d13a-109">Permission type</span></span>                        | <span data-ttu-id="3d13a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d13a-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3d13a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d13a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3d13a-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d13a-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3d13a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d13a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d13a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d13a-114">Not supported.</span></span>                           |
| <span data-ttu-id="3d13a-115">应用</span><span class="sxs-lookup"><span data-stu-id="3d13a-115">Application</span></span>                            | <span data-ttu-id="3d13a-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3d13a-116">Reports.Read.All</span></span>                         |

<span data-ttu-id="3d13a-117">**注意**：对于允许应用程序代表用户读取服务使用情况报告的委派权限，租户管理员必须已为该用户分配适当的 Azure AD 有限管理员角色。</span><span class="sxs-lookup"><span data-stu-id="3d13a-117">**Note**: For delegated permissions to allow apps to read service usage reports on behalf of a user, the tenant administrator must have assigned the user the appropriate Azure AD limited administrator role.</span></span> <span data-ttu-id="3d13a-118">有关更多详细信息，请参阅[授权 For api 以读取 Office 365 使用情况报告](/graph/reportroot-authorization)。</span><span class="sxs-lookup"><span data-stu-id="3d13a-118">For more details, see [Authorization for APIs to read Office 365 usage reports](/graph/reportroot-authorization).</span></span>

## <a name="http-request"></a><span data-ttu-id="3d13a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d13a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(period='{period_value}')
GET /reports/getSkypeForBusinessDeviceUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="3d13a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="3d13a-120">Function parameters</span></span>

<span data-ttu-id="3d13a-121">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3d13a-121">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="3d13a-122">参数</span><span class="sxs-lookup"><span data-stu-id="3d13a-122">Parameter</span></span> | <span data-ttu-id="3d13a-123">类型</span><span class="sxs-lookup"><span data-stu-id="3d13a-123">Type</span></span>   | <span data-ttu-id="3d13a-124">说明</span><span class="sxs-lookup"><span data-stu-id="3d13a-124">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3d13a-125">period</span><span class="sxs-lookup"><span data-stu-id="3d13a-125">period</span></span>    | <span data-ttu-id="3d13a-126">string</span><span class="sxs-lookup"><span data-stu-id="3d13a-126">string</span></span> | <span data-ttu-id="3d13a-127">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3d13a-127">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3d13a-128">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3d13a-128">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3d13a-129">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3d13a-129">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="3d13a-130">date</span><span class="sxs-lookup"><span data-stu-id="3d13a-130">date</span></span>      | <span data-ttu-id="3d13a-131">Date</span><span class="sxs-lookup"><span data-stu-id="3d13a-131">Date</span></span>   | <span data-ttu-id="3d13a-132">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="3d13a-132">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="3d13a-133">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="3d13a-133">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="3d13a-134">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="3d13a-134">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="3d13a-135">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="3d13a-135">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="3d13a-136">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3d13a-136">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3d13a-137">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3d13a-137">The default output type is text/csv.</span></span> <span data-ttu-id="3d13a-138">但是，如果要指定输出类型，则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3d13a-138">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d13a-139">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d13a-139">Request headers</span></span>

| <span data-ttu-id="3d13a-140">名称</span><span class="sxs-lookup"><span data-stu-id="3d13a-140">Name</span></span>          | <span data-ttu-id="3d13a-141">说明</span><span class="sxs-lookup"><span data-stu-id="3d13a-141">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3d13a-142">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d13a-142">Authorization</span></span> | <span data-ttu-id="3d13a-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3d13a-p106">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3d13a-145">响应</span><span class="sxs-lookup"><span data-stu-id="3d13a-145">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3d13a-146">CSV</span><span class="sxs-lookup"><span data-stu-id="3d13a-146">CSV</span></span>

<span data-ttu-id="3d13a-147">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3d13a-147">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3d13a-148">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3d13a-148">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3d13a-149">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="3d13a-149">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3d13a-150">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="3d13a-150">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3d13a-151">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3d13a-151">Report Refresh Date</span></span>
- <span data-ttu-id="3d13a-152">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="3d13a-152">User Principal Name</span></span>
- <span data-ttu-id="3d13a-153">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="3d13a-153">Last Activity Date</span></span>
- <span data-ttu-id="3d13a-154">使用的 Windows</span><span class="sxs-lookup"><span data-stu-id="3d13a-154">Used Windows</span></span>
- <span data-ttu-id="3d13a-155">使用的 Windows 手机</span><span class="sxs-lookup"><span data-stu-id="3d13a-155">Used Windows Phone</span></span>
- <span data-ttu-id="3d13a-156">使用的 Android 手机</span><span class="sxs-lookup"><span data-stu-id="3d13a-156">Used Android Phone</span></span>
- <span data-ttu-id="3d13a-157">使用的 iPhone</span><span class="sxs-lookup"><span data-stu-id="3d13a-157">Used iPhone</span></span>
- <span data-ttu-id="3d13a-158">使用的 iPad</span><span class="sxs-lookup"><span data-stu-id="3d13a-158">Used iPad</span></span>
- <span data-ttu-id="3d13a-159">报表周期</span><span class="sxs-lookup"><span data-stu-id="3d13a-159">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3d13a-160">JSON</span><span class="sxs-lookup"><span data-stu-id="3d13a-160">JSON</span></span>

<span data-ttu-id="3d13a-161">如果成功，此方法在响应`200 OK`正文中返回响应代码和**[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3d13a-161">If successful, this method returns a `200 OK` response code and a **[skypeForBusinessDeviceUsageUserDetail](../resources/skypeforbusinessdeviceusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="3d13a-162">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="3d13a-162">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="3d13a-163">示例</span><span class="sxs-lookup"><span data-stu-id="3d13a-163">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3d13a-164">CSV</span><span class="sxs-lookup"><span data-stu-id="3d13a-164">CSV</span></span>

<span data-ttu-id="3d13a-165">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3d13a-165">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3d13a-166">请求</span><span class="sxs-lookup"><span data-stu-id="3d13a-166">Request</span></span>

<span data-ttu-id="3d13a-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d13a-167">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3d13a-168">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d13a-168">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d13a-169">C#</span><span class="sxs-lookup"><span data-stu-id="3d13a-169">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d13a-170">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d13a-170">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d13a-171">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d13a-171">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3d13a-172">响应</span><span class="sxs-lookup"><span data-stu-id="3d13a-172">Response</span></span>

<span data-ttu-id="3d13a-173">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3d13a-173">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3d13a-174">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3d13a-174">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3d13a-175">JSON</span><span class="sxs-lookup"><span data-stu-id="3d13a-175">JSON</span></span>

<span data-ttu-id="3d13a-176">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3d13a-176">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3d13a-177">请求</span><span class="sxs-lookup"><span data-stu-id="3d13a-177">Request</span></span>

<span data-ttu-id="3d13a-178">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3d13a-178">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3d13a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d13a-179">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getskypeforbusinessdeviceusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getSkypeForBusinessDeviceUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3d13a-180">C#</span><span class="sxs-lookup"><span data-stu-id="3d13a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getskypeforbusinessdeviceusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d13a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d13a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getskypeforbusinessdeviceusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3d13a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d13a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getskypeforbusinessdeviceusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3d13a-183">响应</span><span class="sxs-lookup"><span data-stu-id="3d13a-183">Response</span></span>

<span data-ttu-id="3d13a-184">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3d13a-184">The following is an example of the response.</span></span>

> <span data-ttu-id="3d13a-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3d13a-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
