---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 2e3c83603d6cfaaeed9c9ecfd29ce3b895537057
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267429"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="e797c-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="e797c-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e797c-104">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="e797c-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="e797c-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="e797c-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="e797c-106">权限</span><span class="sxs-lookup"><span data-stu-id="e797c-106">Permissions</span></span>

<span data-ttu-id="e797c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e797c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e797c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e797c-109">Permission type</span></span>                        | <span data-ttu-id="e797c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e797c-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="e797c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e797c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e797c-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e797c-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="e797c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e797c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e797c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e797c-114">Not supported.</span></span>                           |
| <span data-ttu-id="e797c-115">应用</span><span class="sxs-lookup"><span data-stu-id="e797c-115">Application</span></span>                            | <span data-ttu-id="e797c-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="e797c-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="e797c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e797c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="e797c-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="e797c-118">Function parameters</span></span>

<span data-ttu-id="e797c-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="e797c-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="e797c-120">参数</span><span class="sxs-lookup"><span data-stu-id="e797c-120">Parameter</span></span> | <span data-ttu-id="e797c-121">类型</span><span class="sxs-lookup"><span data-stu-id="e797c-121">Type</span></span>   | <span data-ttu-id="e797c-122">说明</span><span class="sxs-lookup"><span data-stu-id="e797c-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="e797c-123">period</span><span class="sxs-lookup"><span data-stu-id="e797c-123">period</span></span>    | <span data-ttu-id="e797c-124">string</span><span class="sxs-lookup"><span data-stu-id="e797c-124">string</span></span> | <span data-ttu-id="e797c-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e797c-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="e797c-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="e797c-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="e797c-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="e797c-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="e797c-128">必需。</span><span class="sxs-lookup"><span data-stu-id="e797c-128">Required.</span></span> |

<span data-ttu-id="e797c-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e797c-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="e797c-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="e797c-130">The default output type is text/csv.</span></span> <span data-ttu-id="e797c-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="e797c-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e797c-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="e797c-132">Request headers</span></span>

| <span data-ttu-id="e797c-133">名称</span><span class="sxs-lookup"><span data-stu-id="e797c-133">Name</span></span>          | <span data-ttu-id="e797c-134">说明</span><span class="sxs-lookup"><span data-stu-id="e797c-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="e797c-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="e797c-135">Authorization</span></span> | <span data-ttu-id="e797c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e797c-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="e797c-138">响应</span><span class="sxs-lookup"><span data-stu-id="e797c-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="e797c-139">CSV</span><span class="sxs-lookup"><span data-stu-id="e797c-139">CSV</span></span>

<span data-ttu-id="e797c-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="e797c-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="e797c-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="e797c-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="e797c-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="e797c-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="e797c-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="e797c-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="e797c-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="e797c-144">Report Refresh Date</span></span>
- <span data-ttu-id="e797c-145">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="e797c-145">Mail For Mac</span></span>
- <span data-ttu-id="e797c-146">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="e797c-146">Outlook For Mac</span></span>
- <span data-ttu-id="e797c-147">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="e797c-147">Outlook For Windows</span></span>
- <span data-ttu-id="e797c-148">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="e797c-148">Outlook For Mobile</span></span>
- <span data-ttu-id="e797c-149">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="e797c-149">Other For Mobile</span></span>
- <span data-ttu-id="e797c-150">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="e797c-150">Outlook For Web</span></span>
- <span data-ttu-id="e797c-151">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="e797c-151">POP3 App</span></span>
- <span data-ttu-id="e797c-152">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="e797c-152">IMAP4 App</span></span>
- <span data-ttu-id="e797c-153">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="e797c-153">SMTP App</span></span>
- <span data-ttu-id="e797c-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="e797c-154">Report Date</span></span>
- <span data-ttu-id="e797c-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="e797c-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="e797c-156">JSON</span><span class="sxs-lookup"><span data-stu-id="e797c-156">JSON</span></span>

<span data-ttu-id="e797c-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="e797c-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e797c-158">示例</span><span class="sxs-lookup"><span data-stu-id="e797c-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="e797c-159">CSV</span><span class="sxs-lookup"><span data-stu-id="e797c-159">CSV</span></span>

<span data-ttu-id="e797c-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="e797c-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="e797c-161">请求</span><span class="sxs-lookup"><span data-stu-id="e797c-161">Request</span></span>

<span data-ttu-id="e797c-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e797c-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="e797c-163">响应</span><span class="sxs-lookup"><span data-stu-id="e797c-163">Response</span></span>

<span data-ttu-id="e797c-164">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="e797c-164">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e797c-165">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e797c-165">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e797c-166">C#</span><span class="sxs-lookup"><span data-stu-id="e797c-166">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e797c-167">Javascript</span><span class="sxs-lookup"><span data-stu-id="e797c-167">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e797c-168">目标-C</span><span class="sxs-lookup"><span data-stu-id="e797c-168">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="e797c-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="e797c-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Mail For Mac,Outlook For Mac,Outlook For Windows,Outlook For Mobile,Other For Mobile,Outlook For Web,POP3 App,IMAP4 App,SMTP App,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="e797c-170">JSON</span><span class="sxs-lookup"><span data-stu-id="e797c-170">JSON</span></span>

<span data-ttu-id="e797c-171">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="e797c-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="e797c-172">请求</span><span class="sxs-lookup"><span data-stu-id="e797c-172">Request</span></span>

<span data-ttu-id="e797c-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e797c-173">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="e797c-174">响应</span><span class="sxs-lookup"><span data-stu-id="e797c-174">Response</span></span>

<span data-ttu-id="e797c-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e797c-175">The following is an example of the response.</span></span>

> <span data-ttu-id="e797c-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e797c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAppUsageUserCounts"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 355

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAppUsageUserCounts)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "mailForMac": 0, 
      "outlookForMac": 0, 
      "outlookForWindows": 0, 
      "outlookForMobile": 0, 
      "otherForMobile": 0, 
      "outlookForWeb": 0, 
      "pop3App": 0, 
      "imap4App": 0, 
      "smtpApp": 0, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="e797c-178">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e797c-178">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e797c-179">C#</span><span class="sxs-lookup"><span data-stu-id="e797c-179">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e797c-180">Javascript</span><span class="sxs-lookup"><span data-stu-id="e797c-180">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e797c-181">目标-C</span><span class="sxs-lookup"><span data-stu-id="e797c-181">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailappusageusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailappusageusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
