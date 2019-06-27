---
title: 'reportRoot: getEmailActivityUserCounts'
description: 可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
ms.openlocfilehash: 97379e9b319be2dcabf29bb7067b846a96f6df6e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35267464"
---
# <a name="reportroot-getemailactivityusercounts"></a><span data-ttu-id="7a7be-103">reportRoot: getEmailActivityUserCounts</span><span class="sxs-lookup"><span data-stu-id="7a7be-103">reportRoot: getEmailActivityUserCounts</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a7be-104">可便于了解正在执行发送、阅读和接收等电子邮件活动的唯一用户数趋势。</span><span class="sxs-lookup"><span data-stu-id="7a7be-104">Enables you to understand trends on the number of unique users who are performing email activities like send, read, and receive.</span></span>

> <span data-ttu-id="7a7be-105">**注意：** 若要详细了解不同的报表视图和名称，请参阅 [Office 365 报表 - 电子邮件活动](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44)。</span><span class="sxs-lookup"><span data-stu-id="7a7be-105">**Note:** For details about different report views and names, see [Office 365 Reports - Email Activity](https://support.office.com/client/Email-activity-1cbe2c00-ca65-4fb9-9663-1bbfa58ebe44).</span></span>

## <a name="permissions"></a><span data-ttu-id="7a7be-106">权限</span><span class="sxs-lookup"><span data-stu-id="7a7be-106">Permissions</span></span>

<span data-ttu-id="7a7be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7a7be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a7be-109">Permission type</span></span>                        | <span data-ttu-id="7a7be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a7be-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :--------------------------------------- |
| <span data-ttu-id="7a7be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a7be-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7a7be-112">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7be-112">Reports.Read.All</span></span>                         |
| <span data-ttu-id="7a7be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a7be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a7be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a7be-114">Not supported.</span></span>                           |
| <span data-ttu-id="7a7be-115">应用</span><span class="sxs-lookup"><span data-stu-id="7a7be-115">Application</span></span>                            | <span data-ttu-id="7a7be-116">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="7a7be-116">Reports.Read.All</span></span>                         |

## <a name="http-request"></a><span data-ttu-id="7a7be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a7be-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } --> 

```http
GET /reports/getEmailActivityUserCounts(period='{period_value}')
```

## <a name="function-parameters"></a><span data-ttu-id="7a7be-118">函数参数</span><span class="sxs-lookup"><span data-stu-id="7a7be-118">Function parameters</span></span>

<span data-ttu-id="7a7be-119">在请求 URL 中，提供以下参数的有效值。</span><span class="sxs-lookup"><span data-stu-id="7a7be-119">In the request URL, provide the following parameter with a valid value.</span></span>

| <span data-ttu-id="7a7be-120">参数</span><span class="sxs-lookup"><span data-stu-id="7a7be-120">Parameter</span></span> | <span data-ttu-id="7a7be-121">类型</span><span class="sxs-lookup"><span data-stu-id="7a7be-121">Type</span></span>   | <span data-ttu-id="7a7be-122">说明</span><span class="sxs-lookup"><span data-stu-id="7a7be-122">Description</span></span>                              |
| :-------- | :----- | :--------------------------------------- |
| <span data-ttu-id="7a7be-123">period</span><span class="sxs-lookup"><span data-stu-id="7a7be-123">period</span></span>    | <span data-ttu-id="7a7be-124">string</span><span class="sxs-lookup"><span data-stu-id="7a7be-124">string</span></span> | <span data-ttu-id="7a7be-125">指定在多长时间内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7a7be-125">Specifies the length of time over which the report is aggregated.</span></span> <span data-ttu-id="7a7be-126">受支持的 {period_value} 值为：D7、D30、D90 和 D180。</span><span class="sxs-lookup"><span data-stu-id="7a7be-126">The supported values for {period_value} are: D7, D30, D90, and D180.</span></span> <span data-ttu-id="7a7be-127">这些值采用格式 D*n*，其中 *n* 表示在多少天内聚合报表。</span><span class="sxs-lookup"><span data-stu-id="7a7be-127">These values follow the format D*n* where *n* represents the number of days over which the report is aggregated.</span></span> <span data-ttu-id="7a7be-128">必需。</span><span class="sxs-lookup"><span data-stu-id="7a7be-128">Required.</span></span> |

<span data-ttu-id="7a7be-129">此方法支持`$format` [OData 查询参数](/graph/query-parameters)来自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a7be-129">This method supports the `$format` [OData query parameter](/graph/query-parameters) to customize the response.</span></span> <span data-ttu-id="7a7be-130">默认输出类型为 text/csv。</span><span class="sxs-lookup"><span data-stu-id="7a7be-130">The default output type is text/csv.</span></span> <span data-ttu-id="7a7be-131">但是, 如果要指定输出类型, 则可以使用 OData $format 查询参数设置为 text/csv 或 application/json。</span><span class="sxs-lookup"><span data-stu-id="7a7be-131">However, if you want to specify the output type, you can use the OData $format query parameter set to text/csv or application/json.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a7be-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a7be-132">Request headers</span></span>

| <span data-ttu-id="7a7be-133">名称</span><span class="sxs-lookup"><span data-stu-id="7a7be-133">Name</span></span>          | <span data-ttu-id="7a7be-134">说明</span><span class="sxs-lookup"><span data-stu-id="7a7be-134">Description</span></span>               |
| :------------ | :------------------------ |
| <span data-ttu-id="7a7be-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a7be-135">Authorization</span></span> | <span data-ttu-id="7a7be-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a7be-p104">Bearer {token}. Required.</span></span> |

## <a name="response"></a><span data-ttu-id="7a7be-138">响应</span><span class="sxs-lookup"><span data-stu-id="7a7be-138">Response</span></span>

### <a name="csv"></a><span data-ttu-id="7a7be-139">CSV</span><span class="sxs-lookup"><span data-stu-id="7a7be-139">CSV</span></span>

<span data-ttu-id="7a7be-140">如果成功，此方法返回 `302 Found` 响应，以重定向到报表的预先验证的下载 URL。</span><span class="sxs-lookup"><span data-stu-id="7a7be-140">If successful, this method returns a `302 Found` response that redirects to a preauthenticated download URL for the report.</span></span> <span data-ttu-id="7a7be-141">可以在响应的 `Location` 头中找到此 URL。</span><span class="sxs-lookup"><span data-stu-id="7a7be-141">That URL can be found in the `Location` header in the response.</span></span>

<span data-ttu-id="7a7be-142">预先验证的下载 URL 的有效时间很短（几分钟），不需要 `Authorization` 头。</span><span class="sxs-lookup"><span data-stu-id="7a7be-142">Preauthenticated download URLs are only valid for a short period of time (a few minutes) and do not require an `Authorization` header.</span></span>

<span data-ttu-id="7a7be-143">CSV 文件包含下面的列标题。</span><span class="sxs-lookup"><span data-stu-id="7a7be-143">The CSV file has the following headers for columns.</span></span>

- <span data-ttu-id="7a7be-144">报表刷新日期</span><span class="sxs-lookup"><span data-stu-id="7a7be-144">Report Refresh Date</span></span>
- <span data-ttu-id="7a7be-145">已发送</span><span class="sxs-lookup"><span data-stu-id="7a7be-145">Send</span></span>
- <span data-ttu-id="7a7be-146">已接收</span><span class="sxs-lookup"><span data-stu-id="7a7be-146">Receive</span></span>
- <span data-ttu-id="7a7be-147">已阅读</span><span class="sxs-lookup"><span data-stu-id="7a7be-147">Read</span></span>
- <span data-ttu-id="7a7be-148">报表日期</span><span class="sxs-lookup"><span data-stu-id="7a7be-148">Report Date</span></span>
- <span data-ttu-id="7a7be-149">报表周期</span><span class="sxs-lookup"><span data-stu-id="7a7be-149">Report Period</span></span>

### <a name="json"></a><span data-ttu-id="7a7be-150">JSON</span><span class="sxs-lookup"><span data-stu-id="7a7be-150">JSON</span></span>

<span data-ttu-id="7a7be-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和**[emailActivitySummary](../resources/emailactivitysummary.md)** 对象。</span><span class="sxs-lookup"><span data-stu-id="7a7be-151">If successful, this method returns a `200 OK` response code and an **[emailActivitySummary](../resources/emailactivitysummary.md)** object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7a7be-152">示例</span><span class="sxs-lookup"><span data-stu-id="7a7be-152">Example</span></span>

### <a name="csv"></a><span data-ttu-id="7a7be-153">CSV</span><span class="sxs-lookup"><span data-stu-id="7a7be-153">CSV</span></span>

<span data-ttu-id="7a7be-154">下面是输出 CSV 的示例。</span><span class="sxs-lookup"><span data-stu-id="7a7be-154">The following is an example that outputs CSV.</span></span>

#### <a name="request"></a><span data-ttu-id="7a7be-155">请求</span><span class="sxs-lookup"><span data-stu-id="7a7be-155">Request</span></span>

<span data-ttu-id="7a7be-156">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a7be-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_csv"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=text/csv
```

#### <a name="response"></a><span data-ttu-id="7a7be-157">响应</span><span class="sxs-lookup"><span data-stu-id="7a7be-157">Response</span></span>

<span data-ttu-id="7a7be-158">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7a7be-158">The following is an example of the response.</span></span>

<!-- { "blockType": "ignored" } --> 

```http
HTTP/1.1 302 Found
Content-Type: text/plain
Location: https://reports.office.com/data/download/JDFKdf2_eJXKS034dbc7e0t__XDe
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7a7be-159">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7a7be-159">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7a7be-160">C#</span><span class="sxs-lookup"><span data-stu-id="7a7be-160">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_csv-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a7be-161">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a7be-161">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_csv-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7a7be-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="7a7be-162">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_csv-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<span data-ttu-id="7a7be-163">执行 302 重定向，下载的 CSV 文件将采用以下架构。</span><span class="sxs-lookup"><span data-stu-id="7a7be-163">Follow the 302 redirection and the CSV file that downloads will have the following schema.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

Report Refresh Date,Send,Receive,Read,Report Date,Report Period
```

### <a name="json"></a><span data-ttu-id="7a7be-164">JSON</span><span class="sxs-lookup"><span data-stu-id="7a7be-164">JSON</span></span>

<span data-ttu-id="7a7be-165">下面是一个返回 JSON 的示例。</span><span class="sxs-lookup"><span data-stu-id="7a7be-165">The following is an example that returns JSON.</span></span>

#### <a name="request"></a><span data-ttu-id="7a7be-166">请求</span><span class="sxs-lookup"><span data-stu-id="7a7be-166">Request</span></span>

<span data-ttu-id="7a7be-167">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7a7be-167">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "reportroot_getemailactivityusercounts_json"
}-->

```http
GET https://graph.microsoft.com/beta/reports/getEmailActivityUserCounts(period='D7')?$format=application/json
```

#### <a name="response"></a><span data-ttu-id="7a7be-168">响应</span><span class="sxs-lookup"><span data-stu-id="7a7be-168">Response</span></span>

<span data-ttu-id="7a7be-169">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7a7be-169">The following is an example of the response.</span></span>

> <span data-ttu-id="7a7be-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7a7be-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailActivitySummary"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailActivitySummary)", 
  "value": [
    {
      "reportRefreshDate": "2017-09-01", 
      "send": 69, 
      "receive": 197, 
      "read": 158, 
      "reportDate": "2017-09-01", 
      "reportPeriod": "7"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7a7be-172">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="7a7be-172">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="7a7be-173">C#</span><span class="sxs-lookup"><span data-stu-id="7a7be-173">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_json-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a7be-174">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a7be-174">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_json-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7a7be-175">目标-C</span><span class="sxs-lookup"><span data-stu-id="7a7be-175">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/reportroot_getemailactivityusercounts_json-Objective-C-snippets.md)]
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
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #csv (score: 5)",
    "Error: /api-reference/beta/api/reportroot-getemailactivityusercounts.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
