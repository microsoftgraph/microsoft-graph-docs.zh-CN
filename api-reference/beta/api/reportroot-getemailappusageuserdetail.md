---
title: 'reportRoot: getEmailAppUsageUserDetail'
description: 获取用户在不同电子邮件应用中执行的活动的详细信息。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: 16785097219a53c78502d72b2f2d06c0c741411e
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36723124"
---
# <a name="reportroot-getemailappusageuserdetail"></a><span data-ttu-id="fc606-103">reportRoot: getEmailAppUsageUserDetail</span><span class="sxs-lookup"><span data-stu-id="fc606-103">reportRoot: getEmailAppUsageUserDetail</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc606-104">获取用户在不同电子邮件应用中执行的活动的详细信息。</span><span class="sxs-lookup"><span data-stu-id="fc606-104">Get details about which activities users performed on the various email apps.</span></span>

> <span data-ttu-id="fc606-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="fc606-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="fc606-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc606-106">Permissions</span></span>

<span data-ttu-id="fc606-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc606-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc606-109">Permission type</span></span>                        | <span data-ttu-id="fc606-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc606-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="fc606-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc606-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc606-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc606-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="fc606-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc606-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc606-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc606-114">Not supported.</span></span>                           |
| <span data-ttu-id="fc606-115">应用</span><span class="sxs-lookup"><span data-stu-id="fc606-115">Application</span></span>                            | <span data-ttu-id="fc606-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="fc606-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="fc606-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc606-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserDetail(period='{period_value}')
GET /reports/getEmailAppUsageUserDetail(date={date_value})
```

## <a name="function-parameters"></a><span data-ttu-id="fc606-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="fc606-118">Function parameters</span></span>

<span data-ttu-id="fc606-119">在请求 URL 中，提供以下任一参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="fc606-119">In the request URL, provide one of the following parameters with a valid value.</span></span>

| <span data-ttu-id="fc606-120">参数</span><span class="sxs-lookup"><span data-stu-id="fc606-120">Parameter</span></span> | <span data-ttu-id="fc606-121">类型</span><span class="sxs-lookup"><span data-stu-id="fc606-121">Type</span></span>   | <span data-ttu-id="fc606-122">说明</span><span class="sxs-lookup"><span data-stu-id="fc606-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="fc606-123">period</span><span class="sxs-lookup"><span data-stu-id="fc606-123">period</span></span>    | <span data-ttu-id="fc606-124">string</span><span class="sxs-lookup"><span data-stu-id="fc606-124">string</span></span> | <span data-ttu-id="fc606-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fc606-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="fc606-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="fc606-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="fc606-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="fc606-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> |
| <span data-ttu-id="fc606-128">date</span><span class="sxs-lookup"><span data-stu-id="fc606-128">date</span></span>      | <span data-ttu-id="fc606-129">Date</span><span class="sxs-lookup"><span data-stu-id="fc606-129">Date</span></span>   | <span data-ttu-id="fc606-130">指定要查看用户在哪个日期执行的任何活动。</span><span class="sxs-lookup"><span data-stu-id="fc606-130">Specifies the date for which you would like to view the users who performed any activity.</span></span> <span data-ttu-id="fc606-131">{date_value} 必须采用格式 YYYY-MM-DD。</span><span class="sxs-lookup"><span data-stu-id="fc606-131">{date_value} must have a format of YYYY-MM-DD.</span></span> <span data-ttu-id="fc606-132">因为此报表的有效期仅为过去 30 天，所以 {date_value} 应为这个范围内的日期。</span><span class="sxs-lookup"><span data-stu-id="fc606-132">As this report is only available for the past 30 days, {date_value} should be a date from that range.</span></span> |

> <span data-ttu-id="fc606-133">**注意：** 需要在 URL 中设置 period 或 date。</span><span class="sxs-lookup"><span data-stu-id="fc606-133">**Note:** You need to set either period or date in the URL.</span></span>

<span data-ttu-id="fc606-134">此方法支持使用 `$format`、`$top` 和 `$skipToken` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fc606-134">This method supports the `$format`, `$top`, and `$skipToken` [OData query parameters](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="fc606-135">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="fc606-135">The default output type is text/csv.</span></span> <span data-ttu-id="fc606-136">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="fc606-136">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc606-137">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc606-137">Request headers</span></span>

| <span data-ttu-id="fc606-138">名称</span><span class="sxs-lookup"><span data-stu-id="fc606-138">Name</span></span>          | <span data-ttu-id="fc606-139">说明</span><span class="sxs-lookup"><span data-stu-id="fc606-139">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="fc606-140">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc606-140">Authorization</span></span> | <span data-ttu-id="fc606-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc606-p105">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="fc606-143">响应</span><span class="sxs-lookup"><span data-stu-id="fc606-143">Response</span></span>

### <a name="csv"></a><span data-ttu-id="fc606-144">CSV</span><span class="sxs-lookup"><span data-stu-id="fc606-144">CSV</span></span>

<span data-ttu-id="fc606-145">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="fc606-145">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="fc606-146">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="fc606-146">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="fc606-147">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="fc606-147">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="fc606-148">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="fc606-148">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="fc606-149">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="fc606-149">Report Refresh Date</span></span>
- <span data-ttu-id="fc606-150">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="fc606-150">User Principal Name</span></span>
- <span data-ttu-id="fc606-151">显示名称</span><span class="sxs-lookup"><span data-stu-id="fc606-151">Display Name</span></span>
- <span data-ttu-id="fc606-152">已删除</span><span class="sxs-lookup"><span data-stu-id="fc606-152">Is Deleted</span></span>
- <span data-ttu-id="fc606-153">删除日期</span><span class="sxs-lookup"><span data-stu-id="fc606-153">Deleted Date</span></span>
- <span data-ttu-id="fc606-154">上次活动日期</span><span class="sxs-lookup"><span data-stu-id="fc606-154">Last Activity Date</span></span>
- <span data-ttu-id="fc606-155">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="fc606-155">Mail For Mac</span></span>
- <span data-ttu-id="fc606-156">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="fc606-156">Outlook For Mac</span></span>
- <span data-ttu-id="fc606-157">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="fc606-157">Outlook For Windows</span></span>
- <span data-ttu-id="fc606-158">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="fc606-158">Outlook For Mobile</span></span>
- <span data-ttu-id="fc606-159">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="fc606-159">Other For Mobile</span></span>
- <span data-ttu-id="fc606-160">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="fc606-160">Outlook For Web</span></span>
- <span data-ttu-id="fc606-161">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="fc606-161">POP3 App</span></span>
- <span data-ttu-id="fc606-162">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="fc606-162">IMAP4 App</span></span>
- <span data-ttu-id="fc606-163">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="fc606-163">SMTP App</span></span>
- <span data-ttu-id="fc606-164">报表周期</span><span class="sxs-lookup"><span data-stu-id="fc606-164">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="fc606-165">JSON</span><span class="sxs-lookup"><span data-stu-id="fc606-165">JSON</span></span>

<span data-ttu-id="fc606-166">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="fc606-166">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserDetail](../resources/emailappusageuserdetail.md)** object in the response body.</span></span>

<span data-ttu-id="fc606-167">此请求的默认页面大小为200个项目。</span><span class="sxs-lookup"><span data-stu-id="fc606-167">The default page size for this request is 200 items.</span></span>

## <a name="example"></a><span data-ttu-id="fc606-168">示例</span><span class="sxs-lookup"><span data-stu-id="fc606-168">Example</span></span>

### <a name="csv"></a><span data-ttu-id="fc606-169">CSV</span><span class="sxs-lookup"><span data-stu-id="fc606-169">CSV</span></span>

<span data-ttu-id="fc606-170">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc606-170">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="fc606-171">请求</span><span class="sxs-lookup"><span data-stu-id="fc606-171">Request</span></span>

<span data-ttu-id="fc606-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc606-172">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc606-173">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fc606-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_csv"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc606-174">C#</span><span class="sxs-lookup"><span data-stu-id="fc606-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc606-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc606-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc606-176">目标-C</span><span class="sxs-lookup"><span data-stu-id="fc606-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc606-177">响应</span><span class="sxs-lookup"><span data-stu-id="fc606-177">Response</span></span>

<span data-ttu-id="fc606-178">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc606-178">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="fc606-179">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="fc606-179">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,User Principal Name,Display Name,Is Deleted,Deleted Date,Last Activity Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Period
```

### <a name="json"></a><span data-ttu-id="fc606-180">JSON</span><span class="sxs-lookup"><span data-stu-id="fc606-180">JSON</span></span>

<span data-ttu-id="fc606-181">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="fc606-181">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="fc606-182">请求</span><span class="sxs-lookup"><span data-stu-id="fc606-182">Request</span></span>

<span data-ttu-id="fc606-183">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc606-183">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fc606-184">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="fc606-184">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageuserdetail_json"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserDetail(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc606-185">C#</span><span class="sxs-lookup"><span data-stu-id="fc606-185">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageuserdetail-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc606-186">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc606-186">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageuserdetail-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc606-187">目标-C</span><span class="sxs-lookup"><span data-stu-id="fc606-187">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageuserdetail-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="fc606-188">响应</span><span class="sxs-lookup"><span data-stu-id="fc606-188">Response</span></span>

<span data-ttu-id="fc606-189">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fc606-189">The following is an example of the response.</span></span>

> <span data-ttu-id="fc606-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc606-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserDetail"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 515

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserDetail)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "userPrincipalName": "userPrincipalName-value", 
      "displayName": "displayName-value", 
      "isDeleted": false, 
      "deletedDate": null, 
      "lastActivityDate": "2017-09-01", 
      "mailForMac": [ ], 
      "outlookForMac": [ ], 
      "outlookForWindows": [ ], 
      "outlookForMobile": [
        "Undetermined"
      ], 
      "otherForMobile": [ ], 
      "outlookForWeb": [
        "Undetermined"
      ], 
      "pop3App": [ ], 
      "imap4App": [ ], 
      "smtpApp": [ ], 
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
