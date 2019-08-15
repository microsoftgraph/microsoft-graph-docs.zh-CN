---
title: 'reportRoot: getEmailAppUsageUserCounts'
description: 获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: apiPageType
ms.openlocfilehash: e7ae6269e69527c5c3230356c31880969028de6a
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36411849"
---
# <a name="reportroot-getemailappusageusercounts"></a><span data-ttu-id="3ad49-103">reportRoot: getEmailAppUsageUserCounts</span><span class="sxs-lookup"><span data-stu-id="3ad49-103">reportRoot: getEmailAppUsageUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ad49-104">获取使用任意电子邮件应用连接到 Exchange Online 的唯一用户数。</span><span class="sxs-lookup"><span data-stu-id="3ad49-104">Get the count of unique users that connected to Exchange Online using any email app.</span></span>

> <span data-ttu-id="3ad49-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件应用使用情况](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d)。</span><span class="sxs-lookup"><span data-stu-id="3ad49-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email apps usage](https://support.office.com/client/Email-apps-usage-c2ce12a2-934f-4dd4-ba65-49b02be4703d).</span></span>

## <a name="permissions"></a><span data-ttu-id="3ad49-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ad49-106">Permissions</span></span>

<span data-ttu-id="3ad49-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ad49-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ad49-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ad49-109">Permission type</span></span>                        | <span data-ttu-id="3ad49-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ad49-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="3ad49-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ad49-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ad49-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ad49-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="3ad49-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ad49-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ad49-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ad49-114">Not supported.</span></span>                           |
| <span data-ttu-id="3ad49-115">应用</span><span class="sxs-lookup"><span data-stu-id="3ad49-115">Application</span></span>                            | <span data-ttu-id="3ad49-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="3ad49-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="3ad49-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ad49-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailAppUsageUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="3ad49-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="3ad49-118">Function parameters</span></span>

<span data-ttu-id="3ad49-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="3ad49-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="3ad49-120">参数</span><span class="sxs-lookup"><span data-stu-id="3ad49-120">Parameter</span></span> | <span data-ttu-id="3ad49-121">类型</span><span class="sxs-lookup"><span data-stu-id="3ad49-121">Type</span></span>   | <span data-ttu-id="3ad49-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ad49-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="3ad49-123">period</span><span class="sxs-lookup"><span data-stu-id="3ad49-123">period</span></span>    | <span data-ttu-id="3ad49-124">string</span><span class="sxs-lookup"><span data-stu-id="3ad49-124">string</span></span> | <span data-ttu-id="3ad49-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3ad49-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="3ad49-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="3ad49-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="3ad49-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="3ad49-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="3ad49-128">必需。</span><span class="sxs-lookup"><span data-stu-id="3ad49-128">Required.</span></span> |

<span data-ttu-id="3ad49-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ad49-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="3ad49-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="3ad49-130">The default output type is text/csv.</span></span> <span data-ttu-id="3ad49-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="3ad49-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ad49-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ad49-132">Request headers</span></span>

| <span data-ttu-id="3ad49-133">名称</span><span class="sxs-lookup"><span data-stu-id="3ad49-133">Name</span></span>          | <span data-ttu-id="3ad49-134">说明</span><span class="sxs-lookup"><span data-stu-id="3ad49-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="3ad49-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ad49-135">Authorization</span></span> | <span data-ttu-id="3ad49-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ad49-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="3ad49-138">响应</span><span class="sxs-lookup"><span data-stu-id="3ad49-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="3ad49-139">CSV</span><span class="sxs-lookup"><span data-stu-id="3ad49-139">CSV</span></span>

<span data-ttu-id="3ad49-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="3ad49-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="3ad49-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="3ad49-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="3ad49-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="3ad49-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="3ad49-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="3ad49-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="3ad49-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="3ad49-144">Report Refresh Date</span></span>
- <span data-ttu-id="3ad49-145">Mail for Mac</span><span class="sxs-lookup"><span data-stu-id="3ad49-145">Mail For Mac</span></span>
- <span data-ttu-id="3ad49-146">Outlook for Mac</span><span class="sxs-lookup"><span data-stu-id="3ad49-146">Outlook For Mac</span></span>
- <span data-ttu-id="3ad49-147">Outlook for Windows</span><span class="sxs-lookup"><span data-stu-id="3ad49-147">Outlook For Windows</span></span>
- <span data-ttu-id="3ad49-148">Outlook for Mobile</span><span class="sxs-lookup"><span data-stu-id="3ad49-148">Outlook For Mobile</span></span>
- <span data-ttu-id="3ad49-149">适用于移动设备的其他应用</span><span class="sxs-lookup"><span data-stu-id="3ad49-149">Other For Mobile</span></span>
- <span data-ttu-id="3ad49-150">Outlook for Web</span><span class="sxs-lookup"><span data-stu-id="3ad49-150">Outlook For Web</span></span>
- <span data-ttu-id="3ad49-151">POP3 应用</span><span class="sxs-lookup"><span data-stu-id="3ad49-151">POP3 App</span></span>
- <span data-ttu-id="3ad49-152">IMAP4 应用</span><span class="sxs-lookup"><span data-stu-id="3ad49-152">IMAP4 App</span></span>
- <span data-ttu-id="3ad49-153">SMTP 应用</span><span class="sxs-lookup"><span data-stu-id="3ad49-153">SMTP App</span></span>
- <span data-ttu-id="3ad49-154">报表日期</span><span class="sxs-lookup"><span data-stu-id="3ad49-154">Report Date</span></span>
- <span data-ttu-id="3ad49-155">报表周期</span><span class="sxs-lookup"><span data-stu-id="3ad49-155">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="3ad49-156">JSON</span><span class="sxs-lookup"><span data-stu-id="3ad49-156">JSON</span></span>

<span data-ttu-id="3ad49-157">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="3ad49-157">If successful, this method returns a `200 OK` response code and an **[emailAppUsageUserCounts](../resources/emailappusageusercounts.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ad49-158">示例</span><span class="sxs-lookup"><span data-stu-id="3ad49-158">Example</span></span>

### <a name="csv"></a><span data-ttu-id="3ad49-159">CSV</span><span class="sxs-lookup"><span data-stu-id="3ad49-159">CSV</span></span>

<span data-ttu-id="3ad49-160">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="3ad49-160">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="3ad49-161">请求</span><span class="sxs-lookup"><span data-stu-id="3ad49-161">Request</span></span>

<span data-ttu-id="3ad49-162">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ad49-162">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3ad49-163">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3ad49-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=text/csv
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ad49-164">C#</span><span class="sxs-lookup"><span data-stu-id="3ad49-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-csv-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ad49-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ad49-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-csv-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ad49-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="3ad49-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-csv-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ad49-167">响应</span><span class="sxs-lookup"><span data-stu-id="3ad49-167">Response</span></span>

<span data-ttu-id="3ad49-168">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3ad49-168">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```

<span data-ttu-id="3ad49-169">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="3ad49-169">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

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

### <a name="json"></a><span data-ttu-id="3ad49-170">JSON</span><span class="sxs-lookup"><span data-stu-id="3ad49-170">JSON</span></span>

<span data-ttu-id="3ad49-171">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="3ad49-171">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="3ad49-172">请求</span><span class="sxs-lookup"><span data-stu-id="3ad49-172">Request</span></span>

<span data-ttu-id="3ad49-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ad49-173">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3ad49-174">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="3ad49-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "reportroot_getemailappusageusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailAppUsageUserCounts(period='D7')?$format=application/json
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ad49-175">C#</span><span class="sxs-lookup"><span data-stu-id="3ad49-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/reportroot-getemailappusageusercounts-json-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ad49-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ad49-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/reportroot-getemailappusageusercounts-json-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ad49-177">目标-C</span><span class="sxs-lookup"><span data-stu-id="3ad49-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/reportroot-getemailappusageusercounts-json-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ad49-178">响应</span><span class="sxs-lookup"><span data-stu-id="3ad49-178">Response</span></span>

<span data-ttu-id="3ad49-179">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3ad49-179">The following is an example of the response.</span></span>

> <span data-ttu-id="3ad49-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ad49-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
